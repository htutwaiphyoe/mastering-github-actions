# Github Actions - The Complete Guide

Course by Maximilian

## 01. Introduction

Github actions => a workflow automation service by Github

basic => essential components => advanced

## 02. What is Github actions

A workflow automation service by Github company, automate all kinds of repository related processes and actions

Github actions handle two features

1. CI/CD => continuous integration & continuous deployment => automate code testing, building and deploying
2. Repository management => automate code review, issues

## 03. Github

Git => an open-source version system => manage source code changes => commit, branch

Github => a cloud-based git repository and services provider

Github actions => Automate CI/CD

## 04. Key Components

Workflows => workflows are attached to repository

Jobs => jobs are included in workflows => define runner (execution environment) => run in parallel by default (can sequential, conditional)

Steps => steps are contained in jobs => shell script or action => custom or third-party actions => executed in order (can conditional )

Workflows > Jobs > Steps

Trigger => runs workflows on certain events

## 05. Workflows in action

repository/.github/workflows/[name].yml

name => workflowName

on => events that trigger workflow runs

workflow_dispatch => manual trigger event

jobs => work to do

runs-on => runner

[github-hosted-runners](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners/about-github-hosted-runners)

steps => step to execute => start with - and key/value pairs

step has name and action to run

run => run on console

## 06. Events (Workflow Triggers)

repository related events => push, pull_request

[events-that-trigger-workflows](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)

github actions runs on github servers, don't run on github repository, so need to get code at first step

[Action for checking out a repo](https://github.com/actions/checkout)

nodejs install => action/setup-node

[setup-node](https://github.com/actions/setup-node)

parallel jobs => default

sequential jobs => needs: jobName / [job1, job2] => if one job fails, other jobs will not run
