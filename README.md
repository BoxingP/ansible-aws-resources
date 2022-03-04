# Project to Create AWS Resources

## Steps

1. Install Ansible

1. Install collections from Ansible Galaxy

   ```
   $ ansible-galaxy collection install -r requirements.yaml
   ```

1. The created AWS resources are dependent on the variables `project` and `deploy_environment`

   The supported code repos list is:

    - [EC2 instances with VPC](https://github.com/BoxingP/ec2-with-vpc)
    - [S3 buckets with IAM](https://github.com/BoxingP/s3-buckets-with-iam)
    - [Filter Out Instances by Tags](https://github.com/BoxingP/filter-out-instances)
    - [Start Stop Instances](https://github.com/BoxingP/start-stop-instances)
    - [Start Stop Policy](https://github.com/BoxingP/start-stop-policy)
    - [Start Stop Scheduler](https://github.com/BoxingP/start-stop-scheduler)
    - [Selenium Automation Test](https://github.com/BoxingP/selenium-auto-test)

1. Run playbook:

   ```
   $ ansible-playbook playbook.yaml --extra-vars "project='{{ project name }}' deploy_environment={{ deploy environment }} repo={{ code repo used }}"
   ```

Then the AWS resources will be created.