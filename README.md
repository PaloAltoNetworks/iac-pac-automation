# Policy-as-Code Automation with Bridgecrew and GitHub Actions

This GitHub Action runs whenever files change in the main branch. It automatically creates, updates or deletes a Bridgecrew custom policy or policies from your Bridgecrew console based on the file changes triggered by the main branch.

This workflow is not ment for production use. Its goal is to provide a way to showcase how one can automate a custom policy lifecycle using Bridgecrew and GitHub Actions.

## Table of Contents

* [Requirements](#requirements)
* [Getting Started](#getting-started)

## Requirements

* Bridgecrew account
* Bridgecrew API token

## Getting started

1. Fork this repo.
2. Navigate to [Bridgecrew's website](https://bridgecrew.io/) and choose get started for free to create a trial account.
3. Once in your Bridgecrew console, navigate to integrations and create an API token.
4. Add the API token to your GitHub repo with the name BC_API_KEY (settings > secrets).
5. Create a new policy (you can use the provided policy GCP_Firewall_RDP_Port_Open.yml or create your own policies).
6. Push your changes to the main branch of the repo.
7. Check the actions tab.
8. In your Bridgecrew console navigate to policies, add GCP to the providers list, add "Created by" and select your username.
