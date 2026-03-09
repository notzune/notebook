in [[Computer networking|computer networking]], a port is a [[Communication endpoint|communication endpoint]] at the software level within an [[Operating system|operating system]], a port is a logical construct that identifies a specific process or a type of network service.

a port is uniquely identified by a number (port number) associated with the combination of a [[Transport layer|transport protocol]] and the network [[IP address]]. the most common transport protocols that use port numbers are the [[Transmission Control Protocol (TCP)]] and the [[User Datagram Protocol (UDP)]].

the port completes the destination and origination addresses of a message within a [[Host (network)|host]] to point to an operating system process. 

specific port numbers are reserved to identify specific services so that an arriving packet can be easily forwarded to a running application, for this purpose port numbers lower than 1024 identify the historically most commonly used services (list of [[List of TCP and UDP ports|well-known port numbers]]).

port numbers are 16-bit [[Integer|unsigned integers]]. port numbers are also known as the socket number, which identifies from which process (application) the sender is sending the message because a host can run several network applications or processes from a single IP address.

ports provide a [[Multiplexing|multiplexing]] service for multiple services or multiple communication sessions at one network address. 