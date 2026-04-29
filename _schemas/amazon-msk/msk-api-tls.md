---
description: <p>Details for client authentication using TLS.</p>
layout: schema
name: Tls
properties_list:
- description: ''
  name: CertificateAuthorityArnList
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-tls-schema.json
slug: msk-api-tls
source_filename: msk-api-tls-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-tls-schema.json\",\n  \"title\": \"Tls\",\n  \"description\": \"\\n            <p>Details for client authentication using TLS.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateAuthorityArnList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"certificateAuthorityArnList\"\n          },\n          \"description\": \"\\n            <p>List of ACM Certificate Authority ARNs.</p>\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"enabled\"\n          },\n          \"description\": \"\\n            <p>Specifies whether\
  \ you want to turn on or turn off TLS authentication.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-tls-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Tls
---
