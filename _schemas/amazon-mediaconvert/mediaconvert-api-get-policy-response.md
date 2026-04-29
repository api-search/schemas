---
description: GetPolicyResponse schema from Amazon MediaConvert API
layout: schema
name: GetPolicyResponse
properties_list:
- description: ''
  name: Policy
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-get-policy-response-schema.json
slug: mediaconvert-api-get-policy-response
source_filename: mediaconvert-api-get-policy-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-get-policy-response-schema.json\",\n  \"title\": \"GetPolicyResponse\",\n  \"description\": \"GetPolicyResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Policy\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"policy\"\n          },\n          \"description\": \"A policy configures behavior that you allow or disallow for your account. For information about MediaConvert policies, see the user guide at http://docs.aws.amazon.com/mediaconvert/latest/ug/what-is.html\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-get-policy-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: GetPolicyResponse
---
