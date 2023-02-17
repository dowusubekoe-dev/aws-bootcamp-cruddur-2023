# Week 0 — Billing and Architecture

## Table of Contents
- [Prerequisite Technologies](#prerequisite)
    - [GitHub](https://github.com/)
    - [Gitpod](https://gitpod.io/)
    - [GitHub Codespaces](https://github.com/features/codespaces)
    - [Momento Account](https://www.gomomento.com/)
        - [Configure CLI](#momento-cli)
    - [Purchase a Domain](https://tld-list.com/)
    - [HoneyComb.io](https://www.honeycomb.io/)
    - [Rollbar Account](https://rollbar.com/)
- [Bootcamp Overview & Intro](#overview)
    1. [Technical Tasks](#tech-tasks)
    <ol type="a">
    1. [Creating AWS Root Account](root-account)
    1. [Creating AWS Account](aws-account)
    1. [Creating New Repository](github-account)
    </ol>
    2. [Business Scenario](#scenario)
- [Homework Hard Assignments](#hha)
    - [Set a Billing alarm (CloudWatch)](#set-alarm)
    - [Set a AWS Budget](#aws-budget)
    - [Generating AWS Credentials](#credentials)
    - [Using CloudShell](#cloudshell)
    - [Conceptual Architecture Diagram](#napkins)
- [Homework Stretch Assignments](#hsa)
    - [Destroy root account credentials, set MFA, IAM roles](#destroy-root)
    - [EventBridge can be used to notify SNS of service health issues](#eventbridge)
    - [Review all pillars in the Well Architected Tool](#well-architected)
    - [Create an architectural diagram of the CI/CD logical pipeline in Lucid Charts](#lucid-chart)
    - [Research technical and service limits to ensure technical flexibility](#tech-services)
- [Resources](#resouces)
    - [Creating an EventBridge rule for AWS Health](https://docs.aws.amazon.com/health/latest/ug/cloudwatch-events-health.html)
    - [System Design for Beginners](https://www.youtube.com/watch?v=m8Icp_Cid5o&t=8s)
    - [Integrate AWS-CLI and ECR in Gitpod](https://www.gitpod.io/guides/integrate-aws-cli-ecr)

### Prerequisite Technologies

#### GitHub
I already have a Github account, which has been active for over 3 years so I was able to create the Grud repository with no issues.I know Github is version control tool that allow you host your code in an online storage and it also helps in collaboration between developers.[ Github](https://github.com)

#### Gitpod
This is kind of something new to me but I did watch some video tutorials and I learnt that it is a cloud development environment that efficiently and securely allow teams to develop a software.[ Gitpod: Always ready to code.](https://www.gitpod.io)

#### GitHub Spaces
I have some experience in GitHub Codespaces because I have been using Github for a while and I used to collaborate with my team on it during my coding bootcamp.

#### Momento
Momento is also another new tool to me and I know it is one of the fastest tools for caching serverless applications. I was able to create the account and also configured the CLI on a Macbook Pro.
##### Configure CLI
```
brew tap momentohq/tap
brew install momento-cli
```
#### Purchase a Domain
For the purchase of the domain, I went to [Cosmotown](https://www.cosmotown.com/) and they has a promotion so I was able to get one at cheaper price.

#### HoneyComb
This tool helps developers to log the sources of issues reported by users interacting with the code with regards to how the application behaves and performs during all the lifecycle stages.

![Feedback on Performance](https://www.honeycomb.io/wp-content/uploads/2022/10/Fast-feedback-on-real-world-performance-v2.svg)
![Feedback on Service Reliability](https://www.honeycomb.io/wp-content/uploads/2022/10/Fast-feedback-on-service-reliability-v2.svg)

#### Rollbar Account
[Rollbar](https://rollbar.com/) provides full coverage across all the applications that your users depend on and love. Automate real-time error response, ensure happier customers, and more productive development teams.

### Bootcamp Overview & Intro

#### Technical Tasks
> ##### a. Creating AWS Root Account
I created a new account by signing up another Gmail account.

![Congratulations](_docs/assets/create-iam.png)

I also set up MFA for the root account by following the [best practices to protect your account](https://docs.aws.amazon.com/accounts/latest/reference/best-practices-root-user.html).
> ##### b. Creating IAM Account
I created an IAM account and added [AdministratorAccess](https://docs.aws.amazon.com/singlesignon/latest/userguide/get-started-assign-account-access-admin-user.html) and [AWSBillingConductorFullAccess](https://docs.aws.amazon.com/singlesignon/latest/userguide/get-started-assign-account-access-admin-user.html) permissions to enable the setting up of Budget and Billing Alarms.In order to also use the AWS CLI, I created the Access key under the user permissions and downloaded the .csv file.

> ##### c. Creating New Repository
I already had a git hub account so I was able create the [aws-bootcamp-cruddur-2023](https://github.com/ExamProCo/aws-bootcamp-cruddur-2023) repository without any issue.

#### Business Scenario
#### Weekly Outcome

### Homework Hard Assignments
#### Set a Billing alarm (CloudWatch)
#### Set a AWS Budget
#### Generating AWS Credentials
#### Using CloudShell


#### Create an architectural diagram of the CI/CD logical pipeline

[Simple IIS Webserver on EC2](https://lucid.app/lucidchart/09d7247f-d701-40a6-92a4-c6dd19c181d4/edit?viewport_loc=113%2C143%2C2002%2C1148%2C0_0&invitationId=inv_6a3f4409-5e1a-4f87-a3fb-e20d0561b243)