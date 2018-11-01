# parsec-terraform
A simple Terraform template and automation tool to build a Parsec Server inside a VPC in AWS in the least expensive availability zone.

This uses a modified Parsec AMI with Steam pre-installed for quick setup. Default password: @w3some.

Only tested on OSX.

## How to use this
1. Clone this repo.
2. [Install Terraform.](https://www.terraform.io/intro/getting-started/install.html)
3. Ensure you have [aws](https://docs.aws.amazon.com/cli/latest/userguide/installing.html) and [jq](https://stedolan.github.io/jq/download/) installed.
4. Run `./bin/parsecadm plan <aws region>` from the root of the repo to see the plan of resources that will be provisioned.
5. Run `./bin/parsecadm apply <aws region>` from the room of the repo to build your Parsec server.
6. Run `./bin/parsecadm destroy` to remove all resources`.
