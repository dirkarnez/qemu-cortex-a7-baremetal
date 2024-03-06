qemu-cortex-a7-baremetal
========================
based on [arm64-kvm-hello-world/bare-metal-aarch64-qemu at main · Lenz-K/arm64-kvm-hello-world](https://github.com/Lenz-K/arm64-kvm-hello-world/tree/main/bare-metal-aarch64-qemu), working

### Notes
- no standard library is available from the compiler
- linux firmware source code shows how to get hardware functionalities
  - [linux/drivers/char/hw_random/iproc-rng200.c at rpi-5.4.y · raspberrypi/linux](https://github.com/raspberrypi/linux/blob/rpi-5.4.y/drivers/char/hw_random/iproc-rng200.c)
### TODOs
- [ ] use CMake
