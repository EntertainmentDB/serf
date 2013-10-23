---
layout: "docs"
page_title: "Commands"
sidebar_current: "docs-commands"
---

# Serf Commands (CLI)

Serf is controlled via a very easy to use command-line interface (CLI).
Serf is only a single command-line application: `serf`. This application
then takes a subcommand such as "agent" or "members". The complete list of
subcommands is in the navigation to the left.

To view a list of the available commands at any time, just run `serf` with
no arguments:

```
$ serf
usage: serf [--version] [--help] <command> [<args>]

Available commands are:
    agent      Runs a Serf agent
    event      Send a custom event through the Serf cluster
    join       Tell Serf agent to join cluster
    members    Lists the members of a Serf cluster
    monitor    Stream logs from a Serf agent
    version    Prints the Serf version
```

To get help for any specific command, pass the `-h` flag to the relevant
subcommand. For example, to see help about the `members` subcommand:

```
$ serf members -h
Usage: serf members [options]

  Outputs the members of a running Serf agent.

Options:

  -rpc-addr=127.0.0.1:7373  RPC address of the Serf agent.
```