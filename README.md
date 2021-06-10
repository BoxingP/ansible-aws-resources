# Project to Create AWS S3 Bucket and Related Accesses

## Steps

1. Install Ansible

1. Install collections from Ansible Galaxy

   ```
   $ ansible-galaxy collection install -r requirements.yaml
   ```

1. Run playbook:

   ```
   $ ansible-playbook playbook.yaml
   ```

Then the AWS S3 bucket and IAM users with related accesses will be created.