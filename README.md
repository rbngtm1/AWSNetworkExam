# AWSNetworkExam


#### How do I implement HA(High Availability) connectivity between my data center and my VPC?
  * https://aws.amazon.com/answers/networking/aws-single-data-center-ha-network-connectivity/
#### Set up VPN connection between AWS VPC and data center and if there is need to implement GRE VPN as standard routing protocol
  * https://docs.aws.amazon.com/whitepapers/latest/aws-vpc-connectivity-options/software-vpn-network-to-amazon.html
#### Link Aggregation Group
  * https://docs.aws.amazon.com/directconnect/latest/UserGuide/lags.html
  * Factors that need to be considered when setting up the LAG group
    * Ensure the existing AWS DC have the same bandwidth
    * Ensure all AWS DC terminates at the same AWS endpoint
#### Monitoring AWS DC connection
  * DC now has a metric available in Cloudwatch and is called "ConnectionState". You can design an alarm whenever the connection is Down. 0 indicates down 1 indicates up.
#### Network conditions that you must meet for direct connect
  * https://docs.aws.amazon.com/directconnect/latest/UserGuide/Welcome.html
  * The network must have support for 802.1Q VLAN
  * The network device must support BGP
  * Auto-negotiation for the port must be disabled for the network device
#### Direct connect pricing (What matters)
  * https://aws.amazon.com/directconnect/pricing/
  * Number of port hours consumed
  * Data transfer from a S3 bucket via a public VIF
  * Data transfer from a VPC via a private VIF
#### To Transfer encrypted large amount of data to S3 
  * Use HTTPS(TLS) for encryption of data in transit
#### How do I enable BFD(Bidirectional Forwarding Detection) for my DX(AWS Direct Connect) connection?
  * https://aws.amazon.com/premiumsupport/knowledge-center/enable-bfd-direct-connect/
  * If you want to route traffic on VPN line in case the Direct connect fails, "In AWS VPN, make AWS Direct Connect as the primary device".
#### Site-to-Site VPN
  * https://docs.aws.amazon.com/vpn/latest/s2svpn/VPC_VPN.html#vpn-route-priority
  * To ensure on-premise devices that are connected to AWS through VPN can reach the resources defined in privated hosted zone, consider using "simple AD" for resolving DNS request.
#### VPC Peering
  * https://docs.aws.amazon.com/vpc/latest/userguide/vpc-peering.html
#### Route 53
  * Active-Active and Active-Passive Failover
    * https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/dns-failover-types.html
  
  
