---
description: GetChannelPolicyResponse schema from Amazon MediaTailor API
layout: schema
name: GetChannelPolicyResponse
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-get-channel-policy-response-schema.json
slug: mediatailor-api-get-channel-policy-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-get-channel-policy-response-schema.json\",\n  \"title\": \"GetChannelPolicyResponse\",\n  \"description\": \"GetChannelPolicyResponse schema from Amazon MediaTailor API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The IAM policy for the channel. IAM policies are used to control access to your channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-get-channel-policy-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetChannelPolicyResponse
---
