# QEMU_CONFIGS

This directory contain all qemu configs for yours vm, generated by -writeconfig option

 
**Directory**: QEMU_CONFIGS

**Description**: Contain all qemu configs, generated by -writeconfig option

**PATH**: $VMMGR_DATA_PATH/QEMU_CONFIGS

***

**Note**: if a qemu config exists for your vm, it will launched using -readconfig. The first time your vm is launched, or when you use 'regen' option, qemu cmdline is generated and end with -writeconfig. So all your vm have a qemu config in this dir. Also, some options never writed by qemu are added in comment in order to reuse it next start.

