Android-ToolChains
================================
This is a repo compatible repository for various toolchains, both kernel and rom.


###Create a Dowload Directory###
```bash
# Make a directory for toolchains
$ mkdir -p ~/Android-Toolchains
# Move into it
$ cd ~/Android-Toolchains
```

###Initializing the Repo and Syncing###
```bash
# Initialize the repo
$ repo init -u https://github.com/HaoZeke/Android-ToolChains -b master
# Sync the repo; use the -j$number flag for threaded downloads.
$ repo sync -j4
```

###Using Kernel Toolchains###
```bash
# Basically just export the cross compiler [modify example for other toolchains]
$ export CROSS_COMPILE=~/Android-Toolchains/UBER/4.8/Kernel/bin/arm-eabi-
```
###Links###
The idea is basically from [Hyper-Toolchain Manifest](https://github.com/hyper-toolchains/KernelToolchain_Manifest "Inspiration").
The usage instructions are from [Sony Developers](http://developer.sonymobile.com/knowledge-base/open-source/open-devices/how-to-build-and-flash-a-linux-kernel/how-to-build-and-flash-a-linux-kernel-from-sony-copyleft-archives/ "Useful").

Finally of course XDA is your friend..
