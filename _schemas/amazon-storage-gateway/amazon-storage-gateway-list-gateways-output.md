---
description: ListGatewaysOutput schema from Amazon Storage Gateway API
layout: schema
name: ListGatewaysOutput
properties_list:
- description: ''
  name: Gateways
  type: object
- description: ''
  name: Marker
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-gateways-output-schema.json
slug: amazon-storage-gateway-list-gateways-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-gateways-output-schema.json\",\n  \"title\": \"ListGatewaysOutput\",\n  \"description\": \"ListGatewaysOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Gateways\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Gateways\"\n        },\n        {\n          \"description\": \"An array of <a>GatewayInfo</a> objects.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"Use the marker in your next request to fetch the next set of gateways in the list. If there are no more gateways to list, this field does not appear in the response.\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-gateways-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListGatewaysOutput
---
