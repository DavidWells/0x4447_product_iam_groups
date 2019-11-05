# 👨‍👩‍👧‍👦 IAM Groups

This stack is here to help you be more organize with your AWS accounts. Over the years we came up with a nice list of IAM Groups that every AWS should have. The groups will make sure it is clear at a glance which user is responsible for what part of AWS.

Before you use this CloudFormation file, make sure to review it to see if the policy that each group has is something that will work for you.

# DISCLAIMER!

This stack is available to anyone at no cost, but on an as-is basis. 0x4447, LLC is not responsible for damages or costs of any kind that may occur when you use the stack. You take full responsibility when you use it.

# Deploy

### CloudFormation

<a target="_blank" href="https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=zer0x4447-IAM-Groups&templateURL=https://s3.amazonaws.com/0x4447-drive-cloudformation/iam_groups.json">
<img align="left" style="float: left; margin: 0 10px 0 0;" src="https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png"></a>

To deploy this stack, all you need to do is click the button to the left and follow the instructions that CloudFormation provides in your AWS Dashboard. Alternatively, you can download the CF file from [here](https://s3.amazonaws.com/0x4447-drive-cloudformation/iam_groups.json).

#### What Will Deploy?

The stack takes advantage of just IAM Groups.

- 5x IAM Groups
    - **Owners**: Owners are like Admins, but just own the company/product.
    - **Root**: Full access to the whole AWS account.
    - **Admins**: All the privilege of a Root, minus the ability to to manage users. Meaning no access to IAM, etc.
    - **Accountants**: Accountants will have access only to the billing section of AWS.
    - **Auditors**: Read only access to specific parts of the site.
    - **Developers**: Can only see CodeBuild logs, can check CodePipeline status and trigger builds if needed, and have access to CodeCommit.
    - **Support**: Mostly read only access to the AWS account to help them debug issues.

# Pricing

IAM Groups doesn't cost anything.

# The End

If you enjoyed this project, please consider giving it a 🌟. And check out our [0x4447 GitHub account](https://github.com/0x4447), where you'll find additional resources you might find useful or interesting.

## Sponsor 🎊

This project is brought to you by 0x4447 LLC, a software company specializing in building custom solutions on top of AWS. Follow this link to learn more: https://0x4447.com. Alternatively, send an email to [hello@0x4447.email](mailto:hello@0x4447.email?Subject=Hello%20From%20Repo&Body=Hi%2C%0A%0AMy%20name%20is%20NAME%2C%20and%20I%27d%20like%20to%20get%20in%20touch%20with%20someone%20at%200x4447.%0A%0AI%27d%20like%20to%20discuss%20the%20following%20topics%3A%0A%0A-%20LIST_OF_TOPICS_TO_DISCUSS%0A%0ASome%20useful%20information%3A%0A%0A-%20My%20full%20name%20is%3A%20FIRST_NAME%20LAST_NAME%0A-%20My%20time%20zone%20is%3A%20TIME_ZONE%0A-%20My%20working%20hours%20are%20from%3A%20TIME%20till%20TIME%0A-%20My%20company%20name%20is%3A%20COMPANY%20NAME%0A-%20My%20company%20website%20is%3A%20https%3A%2F%2F%0A%0ABest%20regards.).

