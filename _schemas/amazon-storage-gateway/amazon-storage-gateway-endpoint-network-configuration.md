---
description: Specifies network configuration information for the gateway associated with the Amazon FSx file system.
layout: schema
name: EndpointNetworkConfiguration
properties_list:
- description: ''
  name: IpAddresses
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-endpoint-network-configuration-schema.json
slug: amazon-storage-gateway-endpoint-network-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-endpoint-network-configuration-schema.json\",\n  \"title\": \"EndpointNetworkConfiguration\",\n  \"description\": \"Specifies network configuration information for the gateway associated with the Amazon FSx file system.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IpAddresses\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressList\"\n        },\n        {\n          \"description\": \"<p>A list of gateway IP addresses on which the associated Amazon FSx file system is available.</p> <note> <p>If multiple file systems are associated with this gateway, this field is required.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-endpoint-network-configuration-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: EndpointNetworkConfiguration
---
