---
title: Using Tanzu Developer Tools for Visual Studio Code
subtitle: Using Tanzu Developer Tools for Visual Studio Code
weight: 2
---

This topic explains how to use the Tanzu Developer Tools extension for Visual Studio Code.
For a more detailed step-by-step walk-through, see Getting Started instructions](../getting-started.md).

# Usage

### Configure extension settings

You must configure the following required Visual Studio Code settings for your app.

To configure Visual Studio Code settings for your app:

  1. Go to `Preferences -> Settings -> Extensions -> Tanzu`.
  2. For Source Image, enter the destination for an image containing source code to be
  published.
  For Local Path, enter the path on the local file system to a directory of code to build.

## Live update


### Starting live update

Right-click your project's `Tiltfile` and select `Tanzu: Live Update Start`

_Or_

Launch the Command Palette (⇧⌘P) and run the `Tanzu: Live Update Start` command.

### Stopping live update

Right-click your project's `Tiltfile` and select `Tanzu: Live Update Stop`

_Or_

Launch the Command Palette (⇧⌘P) and run the `Tanzu: Live Update Stop` command.

> **Note:** When Live Update is stopped, the application will continue to run, but changes will not be present in your running application unless you redeploy it.

### Disabling live update

Launch the Command Palette (⇧⌘P) and run the `Tanzu: Live Update Disable` command, then enter the name of the workload you want to disable live update for.

> **Note:** This will redeploy your workload to the cluster and remove the live update capability.


## Debug

Right-click on your `workload.yaml` and select `Tanzu: Java Debug Start`
