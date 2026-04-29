---
description: Outbound rule of the load balancer.
layout: schema
name: OutboundRulePropertiesFormat
properties_list:
- description: The number of outbound ports to be used for NAT.
  name: allocatedOutboundPorts
  type: integer
- description: Reference to another subresource.
  name: backendAddressPool
  type: object
- description: Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.
  name: enableTcpReset
  type: boolean
- description: The Frontend IP addresses of the load balancer.
  name: frontendIPConfigurations
  type: array
- description: The timeout for the TCP idle connection.
  name: idleTimeoutInMinutes
  type: integer
- description: The protocol for the outbound rule in load balancer.
  name: protocol
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-outbound-rule-properties-format-schema.json
slug: azure-networking-services-outbound-rule-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-outbound-rule-properties-format-schema.json\",\n  \"title\": \"OutboundRulePropertiesFormat\",\n  \"description\": \"Outbound rule of the load balancer.\",\n  \"properties\": {\n    \"allocatedOutboundPorts\": {\n      \"description\": \"The number of outbound ports to be used for NAT.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"backendAddressPool\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"enableTcpReset\": {\n      \"description\": \"Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination.\
  \ This element is only used when the protocol is set to TCP.\",\n      \"type\": \"boolean\"\n    },\n    \"frontendIPConfigurations\": {\n      \"description\": \"The Frontend IP addresses of the load balancer.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"type\": \"array\"\n    },\n    \"idleTimeoutInMinutes\": {\n      \"description\": \"The timeout for the TCP idle connection.\",\n      \"type\": \"integer\"\n    },\n    \"protocol\": {\n      \"description\": \"The protocol for the outbound rule in load balancer.\",\n      \"enum\": [\n        \"Tcp\",\n        \"Udp\",\n        \"All\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"LoadBalancerOutboundRuleProtocol\"\
  \n      }\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"backendAddressPool\",\n    \"frontendIPConfigurations\",\n    \"protocol\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-outbound-rule-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: OutboundRulePropertiesFormat
---
