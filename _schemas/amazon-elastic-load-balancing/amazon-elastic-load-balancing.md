---
description: Represents an Amazon Elastic Load Balancer with its associated configuration, state, listeners, and target groups.
layout: schema
name: Amazon Elastic Load Balancer
properties_list:
- description: The Amazon Resource Name (ARN) of the load balancer
  name: loadBalancerArn
  type: string
- description: The name of the load balancer
  name: loadBalancerName
  type: string
- description: The public DNS name of the load balancer
  name: dnsName
  type: string
- description: The ID of the Amazon Route 53 hosted zone associated with the load balancer
  name: canonicalHostedZoneId
  type: string
- description: The date and time the load balancer was created
  name: createdTime
  type: string
- description: The scheme of the load balancer (internet-facing or internal)
  name: scheme
  type: string
- description: The ID of the VPC for the load balancer
  name: vpcId
  type: string
- description: ''
  name: state
  type: object
- description: The type of load balancer
  name: type
  type: string
- description: The Availability Zones for the load balancer
  name: availabilityZones
  type: array
- description: The IDs of the security groups for the load balancer
  name: securityGroups
  type: array
- description: The type of IP addresses used by the subnets for the load balancer
  name: ipAddressType
  type: string
- description: The ID of the customer-owned address pool
  name: customerOwnedIpv4Pool
  type: string
- description: The listeners configured for the load balancer
  name: listeners
  type: array
- description: The target groups associated with the load balancer
  name: targetGroups
  type: array
- description: Tags assigned to the load balancer
  name: tags
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-schema.json
slug: amazon-elastic-load-balancing
source_filename: amazon-elastic-load-balancing-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/amazon/elasticloadbalancing/load-balancer.json\",\n  \"title\": \"Amazon Elastic Load Balancer\",\n  \"description\": \"Represents an Amazon Elastic Load Balancer with its associated configuration, state, listeners, and target groups.\",\n  \"type\": \"object\",\n  \"required\": [\"loadBalancerArn\", \"loadBalancerName\", \"type\", \"scheme\"],\n  \"properties\": {\n    \"loadBalancerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the load balancer\",\n      \"pattern\": \"^arn:aws:elasticloadbalancing:[a-z0-9-]+:[0-9]{12}:loadbalancer/.+$\"\n    },\n    \"loadBalancerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the load balancer\",\n      \"maxLength\": 32\n    },\n    \"dnsName\": {\n      \"type\": \"string\",\n      \"description\": \"The public DNS name of the load balancer\"\
  \n    },\n    \"canonicalHostedZoneId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Amazon Route 53 hosted zone associated with the load balancer\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the load balancer was created\"\n    },\n    \"scheme\": {\n      \"type\": \"string\",\n      \"description\": \"The scheme of the load balancer (internet-facing or internal)\",\n      \"enum\": [\"internet-facing\", \"internal\"]\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC for the load balancer\",\n      \"pattern\": \"^vpc-[a-f0-9]{8,17}$\"\n    },\n    \"state\": {\n      \"$ref\": \"#/$defs/LoadBalancerState\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of load balancer\",\n      \"enum\": [\"application\", \"network\", \"gateway\"]\n    },\n    \"availabilityZones\": {\n \
  \     \"type\": \"array\",\n      \"description\": \"The Availability Zones for the load balancer\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AvailabilityZone\"\n      }\n    },\n    \"securityGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The IDs of the security groups for the load balancer\",\n      \"items\": {\n        \"type\": \"string\",\n        \"pattern\": \"^sg-[a-f0-9]{8,17}$\"\n      }\n    },\n    \"ipAddressType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of IP addresses used by the subnets for the load balancer\",\n      \"enum\": [\"ipv4\", \"dualstack\"]\n    },\n    \"customerOwnedIpv4Pool\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the customer-owned address pool\"\n    },\n    \"listeners\": {\n      \"type\": \"array\",\n      \"description\": \"The listeners configured for the load balancer\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Listener\"\n      }\n    },\n    \"targetGroups\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"The target groups associated with the load balancer\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TargetGroup\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to the load balancer\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"LoadBalancerState\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the state of a load balancer\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"The state code\",\n          \"enum\": [\"active\", \"provisioning\", \"active_impaired\", \"failed\"]\n        },\n        \"reason\": {\n          \"type\": \"string\",\n          \"description\": \"A description of the state\"\n        }\n      }\n    },\n    \"AvailabilityZone\": {\n      \"type\": \"object\",\n      \"description\": \"Describes an Availability Zone\
  \ for a load balancer\",\n      \"properties\": {\n        \"zoneName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the Availability Zone\"\n        },\n        \"subnetId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the subnet\",\n          \"pattern\": \"^subnet-[a-f0-9]{8,17}$\"\n        },\n        \"loadBalancerAddresses\": {\n          \"type\": \"array\",\n          \"description\": \"The static IP addresses associated with the load balancer\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"ipAddress\": {\n                \"type\": \"string\",\n                \"description\": \"The static IP address\"\n              },\n              \"allocationId\": {\n                \"type\": \"string\",\n                \"description\": \"The allocation ID of the Elastic IP address\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Listener\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Describes a listener for a load balancer\",\n      \"properties\": {\n        \"listenerArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the listener\"\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"description\": \"The protocol for connections from clients\",\n          \"enum\": [\"HTTP\", \"HTTPS\", \"TCP\", \"TLS\", \"UDP\", \"TCP_UDP\", \"GENEVE\"]\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port on which the load balancer is listening\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        },\n        \"sslPolicy\": {\n          \"type\": \"string\",\n          \"description\": \"The security policy that defines supported protocols and ciphers\"\n        },\n        \"certificates\": {\n          \"type\": \"array\",\n          \"description\": \"The SSL server certificates\",\n     \
  \     \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"certificateArn\": {\n                \"type\": \"string\",\n                \"description\": \"The ARN of the certificate\"\n              }\n            }\n          }\n        },\n        \"defaultActions\": {\n          \"type\": \"array\",\n          \"description\": \"The default actions for the listener\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Action\"\n          }\n        }\n      }\n    },\n    \"TargetGroup\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a target group\",\n      \"properties\": {\n        \"targetGroupArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the target group\"\n        },\n        \"targetGroupName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the target group\"\n        },\n        \"protocol\": {\n          \"type\": \"string\",\n          \"\
  description\": \"The protocol to use for routing traffic to the targets\",\n          \"enum\": [\"HTTP\", \"HTTPS\", \"TCP\", \"TLS\", \"UDP\", \"TCP_UDP\", \"GENEVE\"]\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port on which the targets are listening\",\n          \"minimum\": 1,\n          \"maximum\": 65535\n        },\n        \"targetType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of target\",\n          \"enum\": [\"instance\", \"ip\", \"lambda\", \"alb\"]\n        },\n        \"healthCheckEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether health checks are enabled\"\n        },\n        \"healthCheckPath\": {\n          \"type\": \"string\",\n          \"description\": \"The destination for health checks\"\n        }\n      }\n    },\n    \"Action\": {\n      \"type\": \"object\",\n      \"description\": \"Describes an action for a listener or rule\",\n\
  \      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of action\",\n          \"enum\": [\"forward\", \"authenticate-oidc\", \"authenticate-cognito\", \"redirect\", \"fixed-response\"]\n        },\n        \"targetGroupArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the target group\"\n        },\n        \"order\": {\n          \"type\": \"integer\",\n          \"description\": \"The order for the action\"\n        }\n      },\n      \"required\": [\"type\"]\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"description\": \"Describes a resource tag\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The key of the tag\",\n          \"maxLength\": 128\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The value of the tag\",\n          \"maxLength\": 256\n        }\n      },\n\
  \      \"required\": [\"key\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-schema.json
tags:
- Amazon Web Services
- High Availability
- Load Balancing
- Networking
- Scalability
title: Amazon Elastic Load Balancer
---
