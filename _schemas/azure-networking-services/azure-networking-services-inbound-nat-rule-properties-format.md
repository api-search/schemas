---
description: Properties of the inbound NAT rule.
layout: schema
name: InboundNatRulePropertiesFormat
properties_list:
- description: A reference to a private IP address defined on a network interface of a VM. Traffic sent to the frontend port of each of the frontend IP configurations is forwarded to the backend IP.
  name: backendIPConfiguration
  type: object
- description: The port used for the internal endpoint. Acceptable values range from 1 to 65535.
  name: backendPort
  type: integer
- description: Configures a virtual machine's endpoint for the floating IP capability required to configure a SQL AlwaysOn Availability Group. This setting is required when using the SQL AlwaysOn Availability Groups
  name: enableFloatingIP
  type: boolean
- description: Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.
  name: enableTcpReset
  type: boolean
- description: Reference to another subresource.
  name: frontendIPConfiguration
  type: object
- description: The port for the external endpoint. Port numbers for each rule must be unique within the Load Balancer. Acceptable values range from 1 to 65534.
  name: frontendPort
  type: integer
- description: The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.
  name: idleTimeoutInMinutes
  type: integer
- description: The transport protocol for the endpoint.
  name: protocol
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-inbound-nat-rule-properties-format-schema.json
slug: azure-networking-services-inbound-nat-rule-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-inbound-nat-rule-properties-format-schema.json\",\n  \"title\": \"InboundNatRulePropertiesFormat\",\n  \"description\": \"Properties of the inbound NAT rule.\",\n  \"properties\": {\n    \"backendIPConfiguration\": {\n      \"$ref\": \"./networkInterface.json#/definitions/NetworkInterfaceIPConfiguration\",\n      \"description\": \"A reference to a private IP address defined on a network interface of a VM. Traffic sent to the frontend port of each of the frontend IP configurations is forwarded to the backend IP.\",\n      \"readOnly\": true\n    },\n    \"backendPort\": {\n      \"description\": \"The port used for the internal endpoint. Acceptable values range from 1 to 65535.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"enableFloatingIP\"\
  : {\n      \"description\": \"Configures a virtual machine's endpoint for the floating IP capability required to configure a SQL AlwaysOn Availability Group. This setting is required when using the SQL AlwaysOn Availability Groups in SQL server. This setting can't be changed after you create the endpoint.\",\n      \"type\": \"boolean\"\n    },\n    \"enableTcpReset\": {\n      \"description\": \"Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.\",\n      \"type\": \"boolean\"\n    },\n    \"frontendIPConfiguration\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"frontendPort\": {\n      \"description\": \"The port for the external endpoint. Port numbers for each rule must\
  \ be unique within the Load Balancer. Acceptable values range from 1 to 65534.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"idleTimeoutInMinutes\": {\n      \"description\": \"The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"protocol\": {\n      \"description\": \"The transport protocol for the endpoint.\",\n      \"enum\": [\n        \"Udp\",\n        \"Tcp\",\n        \"All\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"TransportProtocol\"\n      }\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\"\
  : true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-inbound-nat-rule-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: InboundNatRulePropertiesFormat
---
