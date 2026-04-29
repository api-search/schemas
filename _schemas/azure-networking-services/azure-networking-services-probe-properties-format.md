---
description: Load balancer probe resource.
layout: schema
name: ProbePropertiesFormat
properties_list:
- description: The interval, in seconds, for how frequently to probe the endpoint for health status. Typically, the interval is slightly less than half the allocated timeout period (in seconds) which allows two full
  name: intervalInSeconds
  type: integer
- description: The load balancer rules that use this probe.
  name: loadBalancingRules
  type: array
- description: 'The number of probes where if no response, will result in stopping further traffic from being delivered to the endpoint. This values allows endpoints to be taken out of rotation faster or slower than '
  name: numberOfProbes
  type: integer
- description: The port for communicating the probe. Possible values range from 1 to 65535, inclusive.
  name: port
  type: integer
- description: The protocol of the end point. If 'Tcp' is specified, a received ACK is required for the probe to be successful. If 'Http' or 'Https' is specified, a 200 OK response from the specifies URI is required
  name: protocol
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The URI used for requesting health status from the VM. Path is required if a protocol is set to http. Otherwise, it is not allowed. There is no default value.
  name: requestPath
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-probe-properties-format-schema.json
slug: azure-networking-services-probe-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-probe-properties-format-schema.json\",\n  \"title\": \"ProbePropertiesFormat\",\n  \"description\": \"Load balancer probe resource.\",\n  \"properties\": {\n    \"intervalInSeconds\": {\n      \"description\": \"The interval, in seconds, for how frequently to probe the endpoint for health status. Typically, the interval is slightly less than half the allocated timeout period (in seconds) which allows two full probes before taking the instance out of rotation. The default value is 15, the minimum value is 5.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"loadBalancingRules\": {\n      \"description\": \"The load balancer rules that use this probe.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n  \
  \      \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"numberOfProbes\": {\n      \"description\": \"The number of probes where if no response, will result in stopping further traffic from being delivered to the endpoint. This values allows endpoints to be taken out of rotation faster or slower than the typical times used in Azure.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"port\": {\n      \"description\": \"The port for communicating the probe. Possible values range from 1 to 65535, inclusive.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"protocol\": {\n      \"description\": \"The protocol of the end point. If 'Tcp' is specified, a received ACK is required for the probe to be successful. If 'Http' or 'Https'\
  \ is specified, a 200 OK response from the specifies URI is required for the probe to be successful.\",\n      \"enum\": [\n        \"Http\",\n        \"Tcp\",\n        \"Https\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProbeProtocol\"\n      }\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n    \"requestPath\": {\n      \"description\": \"The URI used for requesting health status from the VM. Path is required if a protocol is set to http. Otherwise, it is not allowed. There is no default value.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\"\
  : [\n    \"protocol\",\n    \"port\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-probe-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ProbePropertiesFormat
---
