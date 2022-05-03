# Policy-as-Code Automation with Prisma Cloud Code Security and GitHub Actions

This GitHub Action runs whenever files change in the pccs-demo branch. It automatically creates, updates or deletes a Prisma Cloud custom build policy or policies in your Prisma Cloud console based on the file changes triggered by this branch.

This workflow is not ment for production use. Its goal is to provide a way to showcase how one can automate a custom policy lifecycle using Prisma Cloud Code Security and GitHub Actions.

## Table of Contents

* [Requirements](#requirements)
* [Getting Started](#getting-started)

## Requirements

* GitHub account
* Prisma Cloud account
* Prisma Cloud Access Key

## Getting started

1. Fork this repo.
2. If you don't have a Prisma Cloud access key, create one. In Prisma Cloud console, navigate to Settings > Access Control > Access Keys and create a key.
3. Create two secrets in your repo: one called PCS_USER for your access key and one called PCS_PASS for your secret access key.
4. Create a new policy (you can use the provided policies as a template or create your own policies).
6. Push your changes to the pccs-demo branch of the repo.
7. Check the actions tab.
8. In your Prisma Cloud console, navigate to policies, and search for the policy name.
