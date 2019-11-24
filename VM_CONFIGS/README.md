# VM_CONFIGS

This directory contain all you VM definition, used for create a VM.

This command make a copy of a template:

** VMMgr_Launcher create "vm name" "template" **

This will copy <template> in this directory, named <vm name>

Before start the vm, you can edit this file and customize as needed

***

If you plan to create many VMs using the same custom params, you will find
usefull to convert your customized config into template:

copy you customize vm def into Template directory, and change the following:

> script name: %%NAME%%

> ...

> description: Template for %%NAME%%

> ...

> NAME="%%NAME%%"


**%%NAME%%** will be further replaced by the name of your new VM.

You can now create new vm using this template:

** VMMgr_Launcher create "vm name" "new template" **
