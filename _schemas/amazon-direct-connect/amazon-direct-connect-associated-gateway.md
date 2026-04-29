---
description: Information about the associated gateway.
layout: schema
name: AssociatedGateway
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: ownerAccount
  type: object
- description: ''
  name: region
  type: object
provider_name: Amazon Direct Connect
provider_slug: amazon-direct-connect
schema_file: json-schema/amazon-direct-connect-associated-gateway-schema.json
slug: amazon-direct-connect-associated-gateway
source_filename: amazon-direct-connect-associated-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-associated-gateway-schema.json\",\n  \"title\": \"AssociatedGateway\",\n  \"description\": \"Information about the associated gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayIdentifier\"\n        },\n        {\n          \"description\": \"The ID of the associated gateway.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayType\"\n        },\n        {\n          \"description\": \"The type of associated gateway.\"\n        }\n      ]\n    },\n    \"ownerAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OwnerAccount\"\n        },\n        {\n          \"description\"\
  : \"The ID of the Amazon Web Services account that owns the associated virtual private gateway or transit gateway.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Region\"\n        },\n        {\n          \"description\": \"The Region where the associated gateway is located.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-direct-connect/refs/heads/main/json-schema/amazon-direct-connect-associated-gateway-schema.json
tags:
- AWS
- Dedicated Connection
- Direct Connect
- Hybrid Cloud
- Networking
title: AssociatedGateway
---
