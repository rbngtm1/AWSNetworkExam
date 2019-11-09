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
  
  
