a method of implementing a [[Telecommunications network|telecommunications network]] in which two [[Node (networking)|network nodes]] establish a dedicated [[Communication channels|communications channel (circuit)]] through the network before the nodes may communicate. 

the circuit guarantees the full bandwidth of the channel and remains connected for the duration of the communication session. 

connection is established through a dedicated pathway which is a fixed pathway and fixed bandwidth irrespective of the size of the packet and the bandwidth is reserved and constant through the entire communication, the data travels in a continuous stream along the fixed path, leading to inefficiencies. 

the circuit functions as if the nodes were physically connected as with an electrical circuit. in circuit switching, the bit delay is constant during a connection as opposed to [[Packet switching|packet switching]] where packet queues may cause varying and potentially indefinitely long [[End-to-end delay|packet transfer delays]]. 

this is not an issue, as no circuit can be degraded by competing users because it is protected from use by other callers until the circuit is released and a new connection is set up. even if no actual communication is taking place, the channel remains reserved and protected from competing users.

## Inefficiencies

the data travels in a continuous stream along the fixed path, which leads to inefficiencies. the bandwidth is not optimized, we can not change the bandwidth according to the size of the packets, if the packets are of smaller size they still will use the larger bandwidth (doesn't change with packet size).