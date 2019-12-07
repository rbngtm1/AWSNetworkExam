
- https://www.youtube.com/watch?v=SMvom9QjkPk&list=PLlkukGgpsXyvUbJ85RVD7qNJ1mcGKO4_w&index=1

================================================================================================================
#### Direct Connect Requirements
  * Connection Type
    * Dedicated Connections: AWS Direct Connect are provisioned as 1 Gbps or 10 Gbps connections. An AWSDirect Connect connection supports up to 50 Virtual Interfaces(VIF).
    * Hosted Connections: Sub-1GB connections may be provisioned with any AWSDirect Connect partner at 50-500 Mbps, and 1 Gbps, 2 Gbps, 5 Gbps, and 10 Gbps from select partners. A hosted connection supports a single VIF.
    * Hosted VIFS: Newer AWS partners are not allowed to provision Hosted VIFs because of the potential for over subscription, but some existing providers may still have this offering.
  * The network connection for Direct Connect must use single-mode fiber with a 1000 BASE-LX transceiver for a 1 Gigabit Ethernet connection, or a 10GBase-LR transcever for a 10 gigabit Ethernet connection.
  * Auto-negotiation must be disabled on the port and port speed, and full-duplex must be manually configured.
  * 802.1Q VLAN encapsulation is required across the entire connection, including intermediary devices.
  * The router that will be used to connect to the Direct Connect connection must support BGP and BGP MD5 authentication.
  * Bidirectional forwarding is optional
  * A letter of Authorization-Connecting Facility Assignment(LOA-CFA) is required for authorizing the connection into the AWS network.
  * Create the Direct Connect connection in the AWS Console, specifying the name, Direct Connect location, and port speed.
  * Download the LOA-CFA from the AWS Direct Connect console. (Typically withing 72 hours of the request submission), and create the cross-network connection. An AWS Direct Connect partner can help with connecting. Create one LOA per connection, per data cernter. 
  * The LOA-CFA expires after 90 days.
  * Port-hour billing starts 90 days after the connection is created in the AWS console, or when the connection betweeen your router and the AWS Direct Connect endpoint is established. Failure to dlete the connection incurs charges.
  * AWS provides the router configuration necessary for connecting to the AWS network.
  * Hosted connections are purchased from an AWS Direct Connect Partner. The partner provisions the connection for you and authorizes the hosted connection to your account. You must accept the connection before you can use it. 
