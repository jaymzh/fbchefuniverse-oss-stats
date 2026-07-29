# OSS Stats for FB Chef Universe Repos

This repo aims to track stats that affect how the various repos that makeup
the FB Chef Universe are doing.

It leverages [oss-stats](https://github.com/jaymzh/oss-stats) to track those
stats. It assumes oss-stats and this repo are checked out next to each other
on the filesystem.

## tl;dr

While OSS Stats can track all sorts of things, we only use Repo Reports. Those
track **Issue, PR, and CI stats**, and you can see that in
[ci_reports](repo_reports).

## Usage

A weekly CI job runs the report on all universe repos every week on Wednesday,
and the "Waiter" job in Slack then posts it during the Slack meeting Thursday
morning.

You can run a manual report with `./scripts/run_report.sh`, which is a slim
wrapper around the upstream scripts.

For updated information on using these scripts see the [oss-stats
README](https://github.com/jaymzh/oss-stats/blob/main/README.md).
