# TUNED

**Directory**: TUNED

**Description**: Contain a default tuned.conf for hypervisor machine, and an other for guest

**PATH**: $VMMGR_DATA_PATH/TUNED

***

This template is not installed by the script. To use it:

    sudo mkdir /etc/tuned/hypervisor
    sudo cp TUNED/tuned.conf /etc/tuned/hypervisor
    sudo tuned-adm profile hypervisor
