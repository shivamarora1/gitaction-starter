# Project for [GitAction Hackathon 2021](https://dev.to/devteam/join-us-for-the-2021-github-actions-hackathon-on-dev-4hn4).

### Introduction:
This repository contains the GitAction which triggers the work flow(sending notification to slack) whenever a issue with label bug is raised. The issue of type bug are one that require high attention of project owner and required to be fixed as soon as possible.

### My Workflow
- The workflow is triggered whenever `event=issues`  with `types=opened` is happened.
- `If` expression is used to check whether this `issue` contains label `bug` or not. 
- If the above check passes then it stores the various meta values like issue `raiser name`, ` repository url`, `issue url` and `issue title`
- After getting the neccessary data the message on slack channel is sent using `slackapi/slack-github-action@v1.16.0` action.


### Submission Category
`Maintainer Must-Haves`, `Wacky Wildcards`

### YAML File
[LINK](https://github.com/shivamarora1/gitactions-slack-notification-bug-issue-raised/blob/main/.github/workflows/github-actions-demo.yml)

### Additional Resources
- [Learn how to get Slack bot token](https://api.slack.com/bot-users)
- [How to use Git Actions](https://docs.github.com/en/actions)

### Screen shot of alert send on slack

### LICENCE
MIT
