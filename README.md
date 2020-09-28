# flo-devops-test

Goal — check the knowledge of common understanding of high-available application setup in AWS
(using AWS cloud services and Terraform is a must; for deployment you can choose anything you want: helm (preferable), ansible, shell, etc).

You need
- prepare docker image for Wordpress (you can base on https://roots.io/bedrock/ for example or smth else)
- setup multiple wordpress instances in AWS, which provide 100% uptime. Wordpress cluster domain should be "test.wodpress.int" and support zero downtime deployment. Fail of any of node, don't lead to downtime.

*** Extra tasks if previous one easy for you :)
1) Add support of sharing wordpress attachment files via AWS Elastic File System
2) Don't loose open http connections during deployment. Prepare test scenario how you check it
3) Add SSL certificates, to support https on your wordpress domain
4) Create AWS ECR Docker Repository and deploy your custom wordpress image from this registry.
Prepare ADR (Architecture decision record) and attach it to homework with an explanation of why you choose this architecture and toolset.
