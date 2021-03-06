# pingu

[![Build Status](https://github.com/hoffa/pingu/workflows/.github/workflows/workflow.yml/badge.svg)](https://github.com/hoffa/pingu/actions)

pingu lets you know when your process finishes.

Supports Slack and Chime. Works on any POSIX system with `curl`.


## Installation

```shell
curl -Lo /usr/local/bin/pingu https://raw.githubusercontent.com/hoffa/pingu/master/pingu
chmod +x /usr/local/bin/pingu
```

## Usage

```shell
pingu <command>
```

Either `SLACK_WEBHOOK_URL` or `CHIME_WEBHOOK_URL` must be set.

Relevant docs on how to generate webhook URLs:
- [Slack](https://api.slack.com/incoming-webhooks)
- [Chime](https://docs.aws.amazon.com/chime/latest/ug/webhooks.html)

## Example

```shell
pingu docker build -t windows .
```
