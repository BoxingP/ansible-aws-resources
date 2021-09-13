# Project to Create AWS Resources

## Steps

1. Install Ansible

1. Install collections from Ansible Galaxy

   ```
   $ ansible-galaxy collection install -r requirements.yaml
   ```

1. The created AWS resources are dependent on the variable `project`

1. Run playbook:

   ```
   $ ansible-playbook playbook.yaml --extra-vars "project='b2b marketplace' deploy_environment=test"
   ```

Then the AWS resources will be created.