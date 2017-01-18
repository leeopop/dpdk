# ANLAB customized DPDK
~~~~~~~~~~~~~{.sh}
#configure dpdk with
make config T=anlab
~~~~~~~~~~~~~

## Void PMD (void)
void PMD is an extension of null PMD with packet generating options.  
e.g., `--vdev eth_void0,node=0,size=64,protocol=ipv4`

`slow=rw`, `slow=r` option will make vdev's RX/TX to return smaller IO batch sizes.

`protocol=trace,trace=xxx.pcap` replays given pcap file. uncaptured area is filled with random data (changes per every replay loop).


