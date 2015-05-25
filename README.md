# ansible-swsheets
Provisioning and Deployment for [edgebuilder](https://github.com/citizenparker/edgebuilder). This was done against DigitalOcean but any brand-new Ubuntu trusty release should work.

## Usage
1. Clone this repository
2. Run `ansible-galaxy install requirements.txt`
3. Add your server information to an [Ansible inventory file](http://docs.ansible.com/intro_inventory.html) called “production”
4. Make a copy of `group_vars` with appropriate values and encrypting it with [Ansible Vault](https://docs.ansible.com/playbooks_vault.html).
5. Run through the steps in docs/initial_setup.md (Sorry, I haven't bothered to put that initial setup in Ansible yet!)
6. Run `script/provision`
7. When you want to deploy, run `script/deploy`
