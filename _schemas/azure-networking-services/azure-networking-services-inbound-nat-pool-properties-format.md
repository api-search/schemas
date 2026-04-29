---
description: Properties of Inbound NAT pool.
layout: schema
name: InboundNatPoolPropertiesFormat
properties_list:
- description: The port used for internal connections on the endpoint. Acceptable values are between 1 and 65535.
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
- description: The last port number in the range of external ports that will be used to provide Inbound Nat to NICs associated with a load balancer. Acceptable values range between 1 and 65535.
  name: frontendPortRangeEnd
  type: integer
- description: The first port number in the range of external ports that will be used to provide Inbound Nat to NICs associated with a load balancer. Acceptable values range between 1 and 65534.
  name: frontendPortRangeStart
  type: integer
- description: The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.
  name: idleTimeoutInMinutes
  type: integer
- description: The reference to the transport protocol used by the inbound NAT pool.
  name: protocol
  type: object
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-inbound-nat-pool-properties-format-schema.json
slug: azure-networking-services-inbound-nat-pool-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-inbound-nat-pool-properties-format-schema.json\",\n  \"title\": \"InboundNatPoolPropertiesFormat\",\n  \"description\": \"Properties of Inbound NAT pool.\",\n  \"properties\": {\n    \"backendPort\": {\n      \"description\": \"The port used for internal connections on the endpoint. Acceptable values are between 1 and 65535.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"enableFloatingIP\": {\n      \"description\": \"Configures a virtual machine's endpoint for the floating IP capability required to configure a SQL AlwaysOn Availability Group. This setting is required when using the SQL AlwaysOn Availability Groups in SQL server. This setting can't be changed after you create the endpoint.\",\n      \"type\": \"boolean\"\n    },\n    \"\
  enableTcpReset\": {\n      \"description\": \"Receive bidirectional TCP Reset on TCP flow idle timeout or unexpected connection termination. This element is only used when the protocol is set to TCP.\",\n      \"type\": \"boolean\"\n    },\n    \"frontendIPConfiguration\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"frontendPortRangeEnd\": {\n      \"description\": \"The last port number in the range of external ports that will be used to provide Inbound Nat to NICs associated with a load balancer. Acceptable values range between 1 and 65535.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"frontendPortRangeStart\": {\n      \"description\": \"The first port number in the range of external ports that will be used to provide Inbound Nat to NICs associated\
  \ with a load balancer. Acceptable values range between 1 and 65534.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"idleTimeoutInMinutes\": {\n      \"description\": \"The timeout for the TCP idle connection. The value can be set between 4 and 30 minutes. The default value is 4 minutes. This element is only used when the protocol is set to TCP.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"protocol\": {\n      \"$ref\": \"#/definitions/TransportProtocol\",\n      \"description\": \"The reference to the transport protocol used by the inbound NAT pool.\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n     \
  \ }\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"protocol\",\n    \"frontendPortRangeStart\",\n    \"frontendPortRangeEnd\",\n    \"backendPort\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-inbound-nat-pool-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: InboundNatPoolPropertiesFormat
---
