# VMMgr
Bash Script for Qemu/Kvm Virtual Machines Management based on templates and variables.

This is for testing purpose and explore qemu options, for production use, use real tools like LibVirt.

## How to Start?

**This script require some steps before it start working, please see Starting With VMMgr before doing anything!!!!!**


Create a new VM named MyVM based on template 'Linux-base'

**./VMMgr_Launcher create MyVM linux-base**

Customize your VM as needed, the config is found in VM-CONFIGS directory

Then start the VM:

**./VMMgr_Launcher start MyVM**

Insert CDROM using:

**./VMMgr_Launcher load test Fedora31.iso reset**

And connect using SPICE:

**./VMMgr_Launcher connect MyVM spice**


To Stop VM:

**./VMMgr_Launcher stop MyVM**




