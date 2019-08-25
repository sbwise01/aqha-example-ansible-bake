# aqha-example-ansible-bake
A packer based Ansible bake of aqha-example-web-app-role into an AWS machine image.

## Bake steps
1. Run `mkdir -p .galaxy` to create a directory for Ansible galaxy roles
1. Run `ansible-galaxy install --roles-path .galaxy -r requirements.yml` to download Ansible galaxy roles
1. Run `packer build packer.json` to bake AMI
1. Run `rm -rf .galaxy` to cleanup
 