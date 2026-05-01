---
description: UpdateConfigurationRequest schema from Amazon MSK API
layout: schema
name: UpdateConfigurationRequest
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: ServerProperties
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-update-configuration-request-schema.json
slug: msk-api-update-configuration-request
source_filename: msk-api-update-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-configuration-request-schema.json\",\n  \"title\": \"UpdateConfigurationRequest\",\n  \"description\": \"UpdateConfigurationRequest schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"\\n            <p>The description of the configuration revision.</p>\"\n        }\n      ]\n    },\n    \"ServerProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__blob\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serverProperties\"\n          },\n          \"description\": \"\\n        \
  \    <p>Contents of the <filename>server.properties</filename> file. When using the API, you must ensure that the contents of the file are base64 encoded. \\n               When using the AWS Management Console, the SDK, or the AWS CLI, the contents of <filename>server.properties</filename> can be in plaintext.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ServerProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-update-configuration-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateConfigurationRequest
---
