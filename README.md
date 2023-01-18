# Verbose-tribble

In this repository, an example of a Circle CI pipeline for deploying a node.js application to production.

## Pre-requisites

- Setting up CircleCI account
- Installing and registering of a CircleCI [self-hosted runner](https://circleci.com/docs/runner-overview/). 
- Configuring [Slack integration orb](https://circleci.com/docs/slack-orb-tutorial/) on CircleCI.
- Configuring key-pair on self-hosted runner for frictionless SSH communication to production instance.

## How to use

The configuration is enabled by placing the `config.yml` file within a default `.circleci` directory in the node.js repository. Any new commits to the branch automatically run the builds as per the pipeline.

To ensure proper deployement, you should replace 172.1.1.1 with your production server IP or hostname.

For Slack notifications, you may provide your channel ID if this is variable, otherwise the default one will be used.
