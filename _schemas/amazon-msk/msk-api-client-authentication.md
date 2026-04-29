---
description: <p>Includes all client authentication information.</p>
layout: schema
name: ClientAuthentication
properties_list:
- description: ''
  name: Sasl
  type: object
- description: ''
  name: Tls
  type: object
- description: ''
  name: Unauthenticated
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-client-authentication-schema.json
slug: msk-api-client-authentication
source_filename: msk-api-client-authentication-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-client-authentication-schema.json\",\n  \"title\": \"ClientAuthentication\",\n  \"description\": \"\\n            <p>Includes all client authentication information.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sasl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sasl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sasl\"\n          },\n          \"description\": \"\\n            <p>Details for ClientAuthentication using SASL.</p>\"\n        }\n      ]\n    },\n    \"Tls\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tls\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tls\"\n          },\n          \"description\": \"\\n            <p>Details for ClientAuthentication using TLS.</p>\"\
  \n        }\n      ]\n    },\n    \"Unauthenticated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Unauthenticated\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"unauthenticated\"\n          },\n          \"description\": \"\\n            <p>Contains information about unauthenticated traffic to the cluster.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-client-authentication-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClientAuthentication
---
