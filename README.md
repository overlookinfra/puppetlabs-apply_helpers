
# apply_helpers

#### Table of Contents

1. [Description](#description)
2. [Setup - The basics of getting started with apply_helpers](#setup)
3. [Usage - Configuration options and additional functionality](#usage)
4. [Reference - An under-the-hood peek at what the module is doing and how](#reference)

## Description

This module provides helper tasks that are used by the `apply()` functionality in Bolt. These tasks are not intended to be run on their own.

This module allows Bolt plans using `apply()` to be run on a Puppet Enterprise (PE) installation.

## Setup

Install the `apply_helpers` module in PE. Using PE RBAC, grant the ability to run the `apply_helpers::custom_facts` and `apply_helpers::apply_catalog` tasks to those you intend to use this module.

To use Bolt's `apply_prep` function, also install https://github.com/puppetlabs/puppetlabs-puppet_agent's `master` branch.

## Usage

Configure Bolt to [work with PE Orchestrator](https://puppet.com/docs/bolt/latest/bolt_configure_orchestrator.html) and run Bolt commands.

## Reference

This module includes tasks that are invoked automatically by Bolt: `apply_helpers::custom_facts` and `apply_helpers::apply_catalog`. These tasks should not be run on their own.

