# vagrants

## About

My Vagrant files used for rapid provisioning of various development environments.

## Cheat-sheet

Here is a short Vagrant cheatsheet:

- `vagrant init`: Initialize a new Vagrant environment by creating a Vagrantfile.
- `vagrant up`: Start and provision the Vagrant environment.
- `vagrant halt`: Stop the Vagrant environment.
- `vagrant reload`: Restart the Vagrant environment, loads new Vagrantfile configuration.
- `vagrant suspend`: Suspend the machine, saves current running state.
- `vagrant resume`: Resume a suspended Vagrant machine.
- `vagrant status`: Outputs status of the Vagrant machine.
- `vagrant ssh`: Connect to machine via SSH.
- `vagrant destroy`: Stop and delete all traces of the Vagrant machine.
- `vagrant provision`: Provisions the Vagrant machine.
- `vagrant box list`: See a list of all installed boxes on your machine.
- `vagrant box add`: Add a box from the Vagrant Cloud or a URL.
- `vagrant box update`: Update the box for the current environment if updates are available.

Remember, you can always get help on command line by typing `vagrant help`.

## QEMU/KVM Architectures

### Note

Sometimes I use strange CPU's for testing purposes like `EPYC-Milan` or `Opteron_G5`.

You can change them according to your needs or delete/uncomment part:

```rb
      libvirt.cpu_model = "Icelake-Server"
```

### List of CPU's

List of possible X86_64 CPU's:

    486
    pentium
    pentium2
    pentium3
    pentiumpro
    coreduo
    n270
    core2duo
    qemu32
    kvm32
    cpu64-rhel5
    cpu64-rhel6
    qemu64
    kvm64
    Conroe
    Penryn
    Nehalem
    Nehalem-IBRS
    Westmere
    Westmere-IBRS
    SandyBridge
    SandyBridge-IBRS
    IvyBridge
    IvyBridge-IBRS
    Haswell-noTSX
    Haswell-noTSX-IBRS
    Haswell
    Haswell-IBRS
    Broadwell-noTSX
    Broadwell-noTSX-IBRS
    Broadwell
    Broadwell-IBRS
    Skylake-Client
    Skylake-Client-IBRS
    Skylake-Client-noTSX-IBRS
    Skylake-Server
    Skylake-Server-IBRS
    Skylake-Server-noTSX-IBRS
    Cascadelake-Server
    Cascadelake-Server-noTSX
    Icelake-Client
    Icelake-Client-noTSX
    Icelake-Server
    Icelake-Server-noTSX
    Cooperlake
    Snowridge
    athlon
    phenom
    Opteron_G1
    Opteron_G2
    Opteron_G3
    Opteron_G4
    Opteron_G5
    EPYC
    EPYC-IBPB
    EPYC-Rome
    EPYC-Milan
    Dhyana

Possible `aarch64` CPU's:

    a64fx
    arm1026
    arm1136
    arm1136-r2
    arm1176
    arm11mpcore
    arm926
    arm946
    cortex-a15
    cortex-a35
    cortex-a53
    cortex-a57
    cortex-a7
    cortex-a72
    cortex-a76
    cortex-a8
    cortex-a9
    cortex-m0
    cortex-m3
    cortex-m33
    cortex-m4
    cortex-m55
    cortex-m7
    cortex-r5
    cortex-r5f
    max
    neoverse-n1
    pxa250
    pxa255
    pxa260
    pxa261
    pxa262
    pxa270-a0
    pxa270-a1
    pxa270
    pxa270-b0
    pxa270-b1
    pxa270-c0
    pxa270-c5
    sa1100
    sa1110
    ti925t