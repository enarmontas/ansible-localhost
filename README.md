# Ansible Localhost

Ansible playbook for setting up my local development environment on macOS and Fedora.
Here's what it does:
- Setup my Dotfiles / [enarmontas/dotfiles](https://github.com/enarmontas/dotfiles)
- Install and configure Zsh + Oh My Zsh
- Install and configure Vim
- Install Homebrew
- Install Go, Python, Ruby, Terraform and manage them in `rbenv` style
- Install Docker, Vagrant

## Usage
1. Fork this repository and modify to match your desired configuration.

1. Install Ansible

   macOS
   ```
   $ brew install ansible
   ```

   Fedora
   ```
   $ sudo dnf install ansible
   ```

2. Install Ansible requirements

   ```
   $ ansible-galaxy install -r requirements.yml
   ```

3. Run the playbook
   ```
   $ ansible-playbook setup.yml --ask-become-pass
   ```
   Run tasks with specific tag: `-t <tag>`

## To Do
- Remove old `rbenv` and `pyenv` versions
