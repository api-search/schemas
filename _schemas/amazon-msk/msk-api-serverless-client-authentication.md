---
description: <p>Includes all client authentication information.</p>
layout: schema
name: ServerlessClientAuthentication
properties_list:
- description: ''
  name: Sasl
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-serverless-client-authentication-schema.json
slug: msk-api-serverless-client-authentication
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-serverless-client-authentication-schema.json\",\n  \"title\": \"ServerlessClientAuthentication\",\n  \"description\": \"\\n            <p>Includes all client authentication information.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Sasl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerlessSasl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sasl\"\n          },\n          \"description\": \"\\n            <p>Details for ClientAuthentication using SASL.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-serverless-client-authentication-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ServerlessClientAuthentication
---
