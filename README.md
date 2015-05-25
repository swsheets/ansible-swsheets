# ansible-swsheets
Provisioning and Deployment for [swsheets](https://github.com/citizenparker/swsheets). This was done against DigitalOcean but any brand-new Ubuntu trusty release should work.

Even if you aren’t using SWSheets (although how couldn’t you?!), please feel free to use this as an example on provisioning, deploying, and running Elixir Phoenix applications.

## Usage
1. Clone this repository
2. Run `ansible-galaxy install requirements.txt`
3. Add your server information to an [Ansible inventory file](http://docs.ansible.com/intro_inventory.html) called “production”
4. Make a copy of `group_vars` with appropriate values and encrypting it with [Ansible Vault](https://docs.ansible.com/playbooks_vault.html).
5. Run through the steps in docs/initial_setup.md (Sorry, I haven't bothered to put that initial setup in Ansible yet!)
6. Run `script/provision`
7. When you want to deploy, run `script/deploy`

## License

All work within this repo is released under a [Creative Commons Attribution-NonCommercial 3.0 United States](https://creativecommons.org/licenses/by-nc/3.0/us/) license. Essentially you are welcome to do what you like with this as long as you provide attribution and don’t charge for it.