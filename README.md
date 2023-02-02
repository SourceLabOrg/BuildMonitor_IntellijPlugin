# Build Monitor plugin for IntelliJ

[![Version](https://img.shields.io/jetbrains/plugin/v/17440.svg)](https://plugins.jetbrains.com/plugin/17440)
[![Downloads](https://img.shields.io/jetbrains/plugin/d/17440.svg)](https://plugins.jetbrains.com/plugin/17440)

<!-- Plugin description -->
## Build Monitor

### Description
ToolWindow that monitors Workflows/Builds from Github Actions and Buildkite.  Setup profiles which
automatically refresh the status of your builds alerting you when they complete or fail.  Ability to
retry failed builds with one click.

### Cost
The free to use version of the plugin has 100% of the functionality of the paid version, however it
is limited by the number of remote accounts you can configure to one.  And you can only setup two
"monitor profiles."

### Features

#### Free
- Connect to Buildkite to monitor Builds.
- Connect to Github to monitor Workflow actions.
- Configurable fields to be displayed inline with your monitored builds.
- Configurable notifications (poups and sounds) based on the status of monitored builds.
- Configurable filter criteria to limit exactly which builds are monitored.

#### Paid
- Unlimited Accounts.
- Unlimited Monitor Profiles.

---

# Usage

## Adding Buildkite Account

##### Create a new Buildkite API Access Token: [https://buildkite.com/user/api-access-tokens](https://buildkite.com/user/api-access-tokens).
Using your Buildkite account, create a new API access token with the following permissions:
- `GraphQL API` To retrieve users, builds, jobs, and pipelines.
- `Read Pipelines` To list and retrieve details of pipeslines.
- `Read Builds` To list and retrieve details of builds.
- `Modify Builds` To create new, retry failed, and cancel running builds.
- `Read User` To retrieve basic details about users.
- `Read Organizations` Used to list and retrieve details of builds.

##### Add account to Project Settings for Plugin.
<kbd>Settings/Preferences</kbd> > <kbd>Tools</kbd> > <kbd>Build Monitor Accounts</kbd>

1. Click the <kbd>+</kbd> icon and give your new account a name.
2. Select `BUILDKITE` from the <kbd>Type</kbd> field.
3. Paste your API Access Token into to the <kbd>Api Access Token</kbd> field.
4. Click the <kbd>Test Connection</kbd> button to verify everything works.

Skip to instructions below labeled `Setup Build Monitor`

## Adding Github Account

##### Create a new Personal Access Token: [https://github.com/settings/tokens](https://github.com/settings/tokens).
Using your Github account, create a new `Personal Access Token` (classic) with the following permissions:

- `Repository` 
  - `READ` Required to read Workflow Actions.
- `Workflow` 
  - `READ` To list and retrieve details of workflows and workflow actions.
  - `WRITE` To Rerun, retry, and cancel workflows.

<kbd>Settings/Preferences</kbd> > <kbd>Tools</kbd> > <kbd>Build Monitor Accounts</kbd>

1. Click the <kbd>+</kbd> icon and give your new account a name.
2. Select `GITHUB` from the <kbd>Type</kbd> field.
3. Paste your Personal Access Token into to the <kbd>Api Access Token</kbd> field.
4. Click the <kbd>Test Connection</kbd> button to verify everything works.

Skip to instructions below labeled `Setup Build Monitor`

## Setup Build Monitor

## Launch Monitor


Submit BugReports or Feature Requests: [https://github.com/SourceLabOrg/BuildMonitor_IntellijPlugin/issues](https://github.com/SourceLabOrg/BuildMonitor_IntellijPlugin/issues)


<!-- Plugin description end -->

---

## Screen Shots

---

## Installation

- Using IDE built-in plugin system:
  
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>Marketplace</kbd> > <kbd>Search for "Build Monitor"</kbd> >
  <kbd>Install Plugin</kbd>
  
- JetBrains Market Place:

  Download the [latest release](https://plugins.jetbrains.com/plugin/17440-php-data-object-generator) and install it manually using
  <kbd>Settings/Preferences</kbd> > <kbd>Plugins</kbd> > <kbd>⚙️</kbd> > <kbd>Install plugin from disk...</kbd>

---

