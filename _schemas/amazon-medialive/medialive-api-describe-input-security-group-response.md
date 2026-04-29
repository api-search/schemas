---
description: Placeholder documentation for DescribeInputSecurityGroupResponse
layout: schema
name: DescribeInputSecurityGroupResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Inputs
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: WhitelistRules
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-describe-input-security-group-response-schema.json
slug: medialive-api-describe-input-security-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-input-security-group-response-schema.json\",\n  \"title\": \"DescribeInputSecurityGroupResponse\",\n  \"description\": \"Placeholder documentation for DescribeInputSecurityGroupResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"Unique ARN of Input Security Group\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The Id of the Input Security Group\"\n        }\n\
  \      ]\n    },\n    \"Inputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"inputs\"\n          },\n          \"description\": \"The list of inputs currently using this Input Security Group.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSecurityGroupState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"The current state of the Input Security Group.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    },\n    \"WhitelistRules\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/__listOfInputWhitelistRule\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"whitelistRules\"\n          },\n          \"description\": \"Whitelist rules and their sync status\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-describe-input-security-group-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeInputSecurityGroupResponse
---
