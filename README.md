# Instack ManageIQ Pull Request Testing Helper Scripts

## Prerequisities

 * virt-customize from libguestfs-tools package
 * deployed undercloud with instack VM running
 * image for ManageIQ VM

## Usage

To create VM with ManageIQ source code from custom user and branch use:

```sh
./miq_deploy_from -u Ladas -b openstack_infra_ui_for_openstack_components -i miq.qcow2
```

This will prepare `miq.qco2` image, checkout ManageIQ source code from `https://github.com/Ladas/manageiq.git` using `openstack_infra_ui_for_openstack_components` branch.
After first boot VM will have ManageIQ running.
