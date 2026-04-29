---
description: Describes a target group
layout: schema
name: TargetGroup
properties_list:
- description: The Amazon Resource Name (ARN) of the target group
  name: targetGroupArn
  type: string
- description: The name of the target group
  name: targetGroupName
  type: string
- description: The protocol to use for routing traffic to the targets
  name: protocol
  type: string
- description: The port on which the targets are listening
  name: port
  type: integer
- description: The ID of the VPC for the targets
  name: vpcId
  type: string
- description: The protocol to use for health checks
  name: healthCheckProtocol
  type: string
- description: The port to use for health checks
  name: healthCheckPort
  type: string
- description: Whether health checks are enabled
  name: healthCheckEnabled
  type: boolean
- description: The approximate interval between health checks
  name: healthCheckIntervalSeconds
  type: integer
- description: The amount of time to wait for a health check response
  name: healthCheckTimeoutSeconds
  type: integer
- description: The number of consecutive health checks required to consider a target healthy
  name: healthyThresholdCount
  type: integer
- description: The number of consecutive health check failures required to consider a target unhealthy
  name: unhealthyThresholdCount
  type: integer
- description: The destination for health checks on the targets
  name: healthCheckPath
  type: string
- description: The type of target
  name: targetType
  type: string
- description: The ARNs of the load balancers that route traffic to this target group
  name: loadBalancerArns
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-target-group-schema.json
slug: amazon-elastic-load-balancing-target-group
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-target-group-schema.json\",\n  \"title\": \"TargetGroup\",\n  \"description\": \"Describes a target group\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetGroupArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the target group\"\n    },\n    \"targetGroupName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the target group\"\n    },\n    \"protocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol to use for routing traffic to the targets\",\n      \"enum\": [\n        \"HTTP\",\n        \"HTTPS\",\n        \"TCP\",\n        \"TLS\",\n        \"UDP\",\n        \"TCP_UDP\",\n        \"GENEVE\"\n      ]\n    },\n    \"port\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The port on which the targets are listening\"\n    },\n    \"vpcId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the VPC for the targets\"\n    },\n    \"healthCheckProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"The protocol to use for health checks\"\n    },\n    \"healthCheckPort\": {\n      \"type\": \"string\",\n      \"description\": \"The port to use for health checks\"\n    },\n    \"healthCheckEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether health checks are enabled\"\n    },\n    \"healthCheckIntervalSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The approximate interval between health checks\"\n    },\n    \"healthCheckTimeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The amount of time to wait for a health check response\"\n    },\n    \"healthyThresholdCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number\
  \ of consecutive health checks required to consider a target healthy\"\n    },\n    \"unhealthyThresholdCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of consecutive health check failures required to consider a target unhealthy\"\n    },\n    \"healthCheckPath\": {\n      \"type\": \"string\",\n      \"description\": \"The destination for health checks on the targets\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of target\",\n      \"enum\": [\n        \"instance\",\n        \"ip\",\n        \"lambda\",\n        \"alb\"\n      ]\n    },\n    \"loadBalancerArns\": {\n      \"type\": \"array\",\n      \"description\": \"The ARNs of the load balancers that route traffic to this target group\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-target-group-schema.json
tags:
- Amazon Web Services
- AWS
- High Availability
- Load Balancing
- Networking
- Scalability
title: TargetGroup
---
