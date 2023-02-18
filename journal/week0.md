# Week 0 — Billing and Architecture

## Prerequisite Technologies

### GitHub
I already have a Github account, which has been active for over 3 years so I was able to create the Grud repository with no issues.I know Github is version control tool that allow you host your code in an online storage and it also helps in collaboration between developers.[ Github](https://github.com)

### Gitpod
This is kind of something new to me but I did watch some video tutorials and I learnt that it is a cloud development environment that efficiently and securely allow teams to develop a software.[ Gitpod: Always ready to code.](https://www.gitpod.io)

### GitHub Spaces
I have some experience in GitHub Codespaces because I have been using Github for a while and I used to collaborate with my team on it during my coding bootcamp.

### Momento
Momento is also another new tool to me and I know it is one of the fastest tools for caching serverless applications. I was able to create the account and also configured the CLI on a Macbook Pro.
#### Configure CLI
```
brew tap momentohq/tap
brew install momento-cli
```
### Purchase a Domain
For the purchase of the domain, I went to [Cosmotown](https://www.cosmotown.com/) and they has a promotion so I was able to get one at cheaper price.

### HoneyComb
This tool helps developers to log the sources of issues reported by users interacting with the code with regards to how the application behaves and performs during all the lifecycle stages.

![Feedback on Performance](https://www.honeycomb.io/wp-content/uploads/2022/10/Fast-feedback-on-real-world-performance-v2.svg)
![Feedback on Service Reliability](https://www.honeycomb.io/wp-content/uploads/2022/10/Fast-feedback-on-service-reliability-v2.svg)

### Rollbar Account
[Rollbar](https://rollbar.com/) provides full coverage across all the applications that your users depend on and love. Automate real-time error response, ensure happier customers, and more productive development teams.

### Bootcamp Overview & Intro

#### Technical Tasks
> ##### a. Creating AWS Admin Account
I created a new account by signing up another Gmail account.

![Congratulations](_docs/assets/create-iam.png)

I also set up MFA for the root account by following the [best practices to protect your account](https://docs.aws.amazon.com/accounts/latest/reference/best-practices-root-user.html).
> ##### b. Creating IAM Account
I created an IAM account and added [AdministratorAccess](https://docs.aws.amazon.com/singlesignon/latest/userguide/get-started-assign-account-access-admin-user.html) and [AWSBillingConductorFullAccess](https://docs.aws.amazon.com/singlesignon/latest/userguide/get-started-assign-account-access-admin-user.html) permissions to enable the setting up of Budget and Billing Alarms.In order to also use the AWS CLI, I created the Access key under the user permissions and downloaded the .csv file.

> ##### c. Creating New Repository
I already had a git hub account so I was able create the [aws-bootcamp-cruddur-2023](https://github.com/ExamProCo/aws-bootcamp-cruddur-2023) repository without any issue.

#### Business Scenario
I joined the live streaming and listened to the presentation that was done by the support team. The explanations provided helped me better understand the process that a project goes through before it is been published to the public.

#### Generating AWS Credentials
I went through the [AWS documentation](https://docs.aws.amazon.com/keyspaces/latest/devguide/access.credentials.html) on how to create a password for an account. In addition to that, I also created the AWS_ACCESS_KEY and AWS_SECRET_KEY and enabling the console access for the IAM account.

#### Install AWS CLI 
I was able to configure Gitpod with my Github credentials but unfortunately I could not set up AWS on Gitpod because I didn't the values I had to use for the Variables.
For this project, I build an ESXi server, which I also created a VM (Ubuntu 20.0 Desktop) as my development machine. I used the following steps to configure AWS on the Ubuntu VM;
- I installed the AWS CLI via command in **Command Prompt** by goinng through the instructions [AWS CLI install and update](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html)

I initially run the command below
```
aws configure
```
- I entered my Access Key and Secret Key to complete the configuration. Screenshot inserted below.

![Confirmation that AWS CLI is installed](_docs/assets/aws-cli-config.png)

#### Create a Billing alarm
I already have an account with Billing configured so I added the one for Credit and updated the existing budget with three thresholds with notifications been sent to my email address.

#### Create a Budget
The budget was set up some few months back when I created the AWS account.

#### Create an architectural diagram of the CI/CD logical pipeline

[Simple IIS Webserver on EC2](https://lucid.app/lucidchart/09d7247f-d701-40a6-92a4-c6dd19c181d4/edit?viewport_loc=113%2C143%2C2002%2C1148%2C0_0&invitationId=inv_6a3f4409-5e1a-4f87-a3fb-e20d0561b243)