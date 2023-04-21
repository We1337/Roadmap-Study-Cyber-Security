In computer networking, a segment is a unit of data that is encapsulated in a Transport Layer protocol header and sent across a network. Segments are used by Transport Layer protocols such as Transmission Control Protocol (TCP) and User Datagram Protocol (UDP) to transmit data between applications or processes running on different devices.

TCP segments contain a header that includes information such as the source and destination port numbers, sequence number, and acknowledgment number. The payload of a TCP segment is the data being transmitted.

UDP segments also contain a header that includes the source and destination port numbers, but do not include the sequence number or acknowledgment number. The payload of a UDP segment is the data being transmitted.

Segments are created by the sender's Transport Layer and are sent to the receiver's Transport Layer. The receiver's Transport Layer then reassembles the segments into the original data stream and passes it to the receiving application.

Segments can be fragmented by routers if they are too large to be transmitted over a network in a single packet. The fragments are then reassembled by the receiver's Transport Layer. However, fragmentation can have a negative impact on network performance and should be avoided whenever possible.

Overall, segments are an important unit of data used by Transport Layer protocols to provide reliable and efficient data transfer between applications running on different devices.