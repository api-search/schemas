---
description: Information about a connection.
layout: schema
name: ConnectionDetails
properties_list:
- description: ''
  name: ClientPublicKey
  type: object
- description: ''
  name: ServerPublicKey
  type: object
- description: ''
  name: ServerEndpoint
  type: object
- description: ''
  name: ClientTunnelAddress
  type: object
- description: ''
  name: ServerTunnelAddress
  type: object
- description: ''
  name: AllowedIps
  type: object
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-connection-details-schema.json
slug: openapi-connection-details
source_filename: openapi-connection-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-connection-details-schema.json\",\n  \"title\": \"ConnectionDetails\",\n  \"description\": \" Information about a connection. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WireGuardPublicKey\"\n        },\n        {\n          \"description\": \" The public key of the client. \"\n        }\n      ]\n    },\n    \"ServerPublicKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WireGuardPublicKey\"\n        },\n        {\n          \"description\": \" The public key of the server. \"\n        }\n      ]\n    },\n    \"ServerEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerEndpoint\"\n        },\n        {\n       \
  \   \"description\": \" The endpoint for the server. \"\n        }\n      ]\n    },\n    \"ClientTunnelAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDR\"\n        },\n        {\n          \"description\": \" The client tunnel address. \"\n        }\n      ]\n    },\n    \"ServerTunnelAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDR\"\n        },\n        {\n          \"description\": \" The server tunnel address. \"\n        }\n      ]\n    },\n    \"AllowedIps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CIDRList\"\n        },\n        {\n          \"description\": \" The allowed IP addresses. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-connection-details-schema.json
tags:
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: ConnectionDetails
---
