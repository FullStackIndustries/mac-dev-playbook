## Installation

1. Ensure Apple's command line tools are installed (`xcode-select --install` to launch the installer).
2. Install Rosetta 2 by running the command `sudo softwareupdate --install-rosetta`. On Apple Silicon Macs, this will allow installation of software without a native ARM port.
3. [Install Ansible](https://docs.ansible.com/ansible/latest/installation_guide/index.html):

   1. Run the following command to add Python 3 to your $PATH: `export PATH="$HOME/Library/Python/3.9/bin:/opt/homebrew/bin:$PATH"`
   2. Upgrade Pip: `sudo pip3 install --upgrade pip`
   3. Install Ansible: `pip3 install ansible`

4. Clone or download this repository to your local drive.
5. Run `ansible-galaxy install -r requirements.yml` inside this directory to install required Ansible roles.
6. Run `ansible-playbook main.yml --ask-become-pass` inside this directory. Enter your macOS account password when prompted for the 'BECOME' password.
