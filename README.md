# cloudps1: Cloud provider prompt for bash

A script that lets you add the current cloud providers account
and region configured via the cloud providers CLI to your
Bash prompt strings (i.e. the `$PS1`).

## History

Customers today work with many cloud providers like Amazon Web Services (AWS), Google Cloud (GCP), and Microsoft Azure and each cloud provider has their own command-line client (CLI) to interact with their services/APIs.  Many Customers have multiple accounts as this is best practice for physical separate of resources.  For example, a Customer might have two accounts in AWS.  One is for production workloads and the other for development purposes  Many of the cloud providers, via the CLI, allow you to create “profiles” so you can interact with different accounts (AWS), or projects (GCP), or subscriptions (Azure).  These profiles are stored in files on the Customers computer that direct them on how to connect to the targeted account(s), project(s), or subscription(s) .

For example, AWS stores a credential file and a configuration file that the AWS CLI uses to perform actions on a customer’s account.  These files contain information on the AWS region to perform work out of, access keys to use for that account, and the secret credential file to use to connect to targeted region.  The Customer can setup multiple “profiles” within the credential and configuration file to connect to multiple AWS accounts.  After creating the profiles, the Customer has to specify a certain command line argument that indicates the profile name and the command they would like to run.
