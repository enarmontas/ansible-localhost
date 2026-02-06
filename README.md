# Ansible Localhost

Ansible playbook for setting up my local development environment on macOS.
Here's what it does:
- Setup my Dotfiles / [enarmontas/dotfiles](https://github.com/enarmontas/dotfiles)
- Install and configure Zsh + Oh My Zsh
- Install and configure Vim
- Install Homebrew and packages

## Usage
1. Fork this repository and modify to match your desired configuration.

1. Install Ansible using Python package manager

   ```
   $ pip3 install ansible
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
