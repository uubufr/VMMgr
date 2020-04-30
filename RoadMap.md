# ROADMAP

## Bugs:

- Set_Service_Listen: all cases are not yet enough tested, this may not work properly. Only bridge with fixed IP, and new port for services work correctly.

- STOPWAIT: work fine but ignore reverse order.

- Groups: when WAIT=yes, we use "systemctl -H <hostname> is-system-running" to test if vm is correctly started, but 1. this implies ssh keys in place, and 2. we don't now on wich interface sshd is listenning.

## ToDo:

- SPICE: spice cac, spice virgl, kiosk mode and ssh tunnel

- VNC: sasl and acl, ssh tunnel

- AUDIO: qemu now use audiodev instead of QEMU_AUDIO_DRV

- MICROVM

- Block Device: be able to attach block devices (nfs, glusterfs, etc.)

- Snapshots

- Migrations

- IPMI

- virgl: be able to add a physical graphical card a vm and use spice virgl=on

- Audit/Performances: be able to evaluate and compare various options and features

- Security: be able to use cgroups features to limit ressources accès (using systemd and/or in a docker container)

- LUKS: be able to create encrypted volumes

- Tuned: tuned for guest

