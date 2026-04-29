---
description: PutChannelPolicyRequest schema from Amazon MediaTailor API
layout: schema
name: PutChannelPolicyRequest
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-put-channel-policy-request-schema.json
slug: mediatailor-api-put-channel-policy-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-put-channel-policy-request-schema.json\",\n  \"title\": \"PutChannelPolicyRequest\",\n  \"description\": \"PutChannelPolicyRequest schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"Adds an IAM role that determines the permissions of your channel.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Policy\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-put-channel-policy-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: PutChannelPolicyRequest
---
