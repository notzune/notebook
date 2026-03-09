in a [[Computer network|network]] based on [[Packet switching|packet switching]], transmission delay (aka [[Store-and-forward delay|store-and-forward delay]], [[Serialization delay|serialization delay]], and [[Packetization delay|packetization delay]]) is the amount of time required to push all the packet's bits into the wire; i.e. the data-rate of the link.

is a function of the packet's length and has nothing to do with the distance between the two [[Node (networking)|nodes]]. this delay is proportional to the packet's length in [[Bit|bits]] and is given by the formula:

$$
D_T=N/R\text{ seconds}
$$

where

- $D_T$ is the transmission delay (in seconds)
- $N$ is the number of bits
- $R$ is the rate of transmission (bits per second)

most modern connections are measured in megabits per second (Mbps) or even gigabits (Gbps).

most packet switched networks use store-and-forward transmission at the input of the link. the switch will receive (save) the entire packet to the [[Data buffer|buffer]] and check it for [[Cyclic redundancy check (CRC)|CRC]] errors or other problems before sending the first bit to the outbound link.

***see [[Network delay|network delay]]***