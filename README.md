# dpdk-devname

Print info about DPDK ports on a system.

## build
clone into dpdk/examples
```
meson setup -Dexamples=devname [other options] build
cd build && ninja && ninja install
```

## usage:
```
$ ./build/examples/dpdk-devname
> EAL: Detected CPU lcores: 32
> EAL: Detected NUMA nodes: 1
> EAL: Detected static linkage of DPDK
> EAL: Multi-process socket /var/run/dpdk/rte/mp_socket
> EAL: Selected IOVA mode 'PA'
> EAL: Probe PCI driver: net_mana (1414:ba) device: 7870:00:00.0 (socket 0)
> mana_init_once(): MP INIT PRIMARY
> TELEMETRY: No legacy callbacks, legacy socket not created
> dpdk-devname found port:0 driver:net_mana eth_dev_info_name:7870:00:00.0 get_name_by_port_name:7870:00:00.0_port1 owner_id:0x0000000000000000 owner_name:
> dpdk-devname found port:1 driver:net_mana eth_dev_info_name:7870:00:00.0 get_name_by_port_name:7870:00:00.0_port2 owner_id:0x0000000000000000 owner_name:
```
