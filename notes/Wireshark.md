
1. `ip.addr == YOUR_IPv4_ADDRESS and tcp`

to get IP, on Windows go to command prompt -> `ipconfig`

on Mac, go to terminal -> `ipconfig getifaddr en0`

2. `tcp.flags.syn == 1 and tcp.flags.ack == 1`

`syn` means going from the sender that sends the data, receiver establishes the connection and says I will send you the data, then `ack` means the sender acknowledges the connection and the above filter is all about setting the connection.

3. go to "Statistics" (top menu) -> go to TCP stream graphs -> go to round trip time and look at the graph
the [[Round-trip delay|round trip time]] shows us the delay in the transmission due to the three way handshake between the sender of the request for the packet (source) and the server (destination) and if this handshake gets delayed, the packet transmission gets delayed, and if the network is congested, there will be more delays in the packet transmission. when the graph of the round trip time.