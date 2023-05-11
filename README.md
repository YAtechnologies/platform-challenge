# Yassir Platform Engineering Take Home Challenge

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/YAtechnologies/platform-challenge)

**Note**: Do not **fork** this repository. Instead:
- Clone it locally. 
- Create a new **private** repository on Github and invite your interviewers (Github usernames will be provided to you). 
- We do not accept pull requests.

This repository acts as a boilerplate to get you started tackling Yassir's platform engineering challenge.

The stack used here is close to what we use for Infrastructure As Code. Mainly:

- [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli).
- [CDK for Terraform](https://developer.hashicorp.com/terraform/tutorials/cdktf/cdktf-install).
- Typescript as the IaC language of choice.
- A [monorepo](https://monorepo.tools/) managed with [pnpm](https://pnpm.io/).

Once you have the above-mentioned tools installed you can run `pnpm install` to install the npm/Typescript dependencies.

For your convenience, we also provided a `.gitpod.yml` file so you can have an already setup environment on GitPod. Simply click "Open in Gitpod" button above. 

## About the challenge
The challenge is about showcasing your ability to implement and manage infrastructure using code. You'll need to use Hashicups.

[Hashicups](https://registry.terraform.io/providers/hashicorp/hashicups/latest/docs) is a fictional Terraform provider. It does not provision real infrastructure (like AWS or GCP), but instead resources are represented as coffee
orders in a coffee-shop. The idea is to mimic cloud-providers with a simple, fun API, without having to deal with cloud providers registrations, accounts or billing for our candidates.

The gist of the work is mostly translating the [CRUD operations](https://developer.hashicorp.com/terraform/tutorials/providers/provider-use) from plain Terraform to CDKTF.


## The deliverable
The final output should be this repository updated with your code, configs and setup. We should be able to:
- Run `pnpm install` for all required/new dependencies.
- A way or a command to run Hashicups APIs locally. We recommend using docker compose for that. The GitPod environment already has docker compose installed for you.
- `README.md` file updated, or a `help` file included on how to provision the infrastructure using Hashicups.
- Be able to provision the CRUD operation for the coffee-shop. The Infrastructure as Code should go under `packages/iac`.
- A way to destroy/cleanup the infrastructure.
- All using cdktf, not plain terraform (no HCL).
- Bonus points for using [Constructs](https://developer.hashicorp.com/terraform/cdktf/concepts/constructs) and [CDKTF best practices](https://developer.hashicorp.com/terraform/cdktf/create-and-deploy/best-practices).
- A simple testing suite that makes sure CDKTF synthesizes the infrastructure correctly. 

### Having troubles?
If you're encountering any troubles, feel free to send an email to `platform@yassir.com`.
