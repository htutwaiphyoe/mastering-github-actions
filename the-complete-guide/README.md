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
