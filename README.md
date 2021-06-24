# Ansible Localhost

## Usage
1. Install Ansible

   macOS
   ```
   brew install ansible
   ```

2. Install Ansible requirements

   ```
   ansible-galaxy install -r requirements.yml
   ```

3. Run the playbook
   ```
   ansible-playbook setup.yml --ask-become-pass
   ```
   Run tasks with specific tag: `-t <tag>`

## To Do
- Homebrew dependencies for `rbenv` and `pyenv`
- Remove old `rbenv` and `pyenv` versions
- Terraform
- Golang
- Move hardcoded values to vars file
