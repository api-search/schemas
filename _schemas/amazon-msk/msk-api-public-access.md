---
description: Public access control for brokers.
layout: schema
name: PublicAccess
properties_list:
- description: ''
  name: Type
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-public-access-schema.json
slug: msk-api-public-access
source_filename: msk-api-public-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-public-access-schema.json\",\n  \"title\": \"PublicAccess\",\n  \"description\": \"Public access control for brokers.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"\\n            <p>The value DISABLED indicates that public access is turned off. SERVICE_PROVIDED_EIPS indicates that public access is turned on.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-public-access-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PublicAccess
---
