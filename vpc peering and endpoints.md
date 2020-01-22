# VPC peering
  * VPC peering cannot be established for IPv6 CPDR block with overlapping IPv4 CIDR block
  
# Endpoints
## Interface Endpoints
  * can be used to connect from subnets in VPC to various AWS services like Amazon SQS directly without internet. With Interface endpoint, servers from on-premise locations will be able to connect to AWS resources only when On-Prem location are connecting via AWS Direct Connect links.
## Gateway Endpoints 
  * gateway endpoints are free whereas interface endpoint are charged per hour and per GB processed.
    * Endpoint for s3
    * Endpoint for DynamoDB
    
## VPC Endpoint Services (AWS Private Link)
  * https://docs.aws.amazon.com/vpc/latest/userguide/endpoint-service.html
