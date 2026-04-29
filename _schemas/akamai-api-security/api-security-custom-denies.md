---
description: Contains details about custom deny actions.
layout: schema
name: custom-denies
properties_list:
- description: A list of custom deny actions in this configuration version.
  name: ratePolicies
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-custom-denies-schema.json
slug: api-security-custom-denies
source_filename: api-security-custom-denies-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-custom-denies-schema.json\",\n  \"title\": \"custom-denies\",\n  \"description\": \"Contains details about custom deny actions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ratePolicies\": {\n      \"description\": \"A list of custom deny actions in this configuration version.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"description\": \"Contains details about a custom deny action.\",\n        \"properties\": {\n          \"description\": {\n            \"description\": \"Describes the custom deny action.\",\n            \"type\": \"string\"\n          },\n          \"id\": {\n            \"description\": \"__Read-only__ Uniquely identifies the custom deny action.\",\n            \"readOnly\": true,\n            \"type\": \"string\"\n         \
  \ },\n          \"name\": {\n            \"description\": \"The name you assigned to the custom deny action.\",\n            \"type\": \"string\"\n          },\n          \"parameters\": {\n            \"description\": \"Describes the custom deny parameters.\",\n            \"items\": {\n              \"additionalProperties\": false,\n              \"description\": \"Contains a list of parameters for the custom deny action. These parameters are not the same type of parameters you usually include in the path of a request.\",\n              \"properties\": {\n                \"displayName\": {\n                  \"description\": \"The description of the custom deny parameter.\",\n                  \"type\": \"string\"\n                },\n                \"name\": {\n                  \"description\": \"The custom deny parameter you choose instead of the Akamai default response. For available values, see [Deny name values](https://techdocs.akamai.com/application-security/reference/deny-name-values).\"\
  ,\n                  \"enum\": [\n                    \"response_status_code\",\n                    \"prevent_browser_cache\",\n                    \"response_content_type\",\n                    \"response_body_content\",\n                    \"response_header_name\",\n                    \"response_header_value\",\n                    \"custom_deny_hostname\",\n                    \"custom_deny_path\",\n                    \"include_true_ip\",\n                    \"include_reference_id\"\n                  ],\n                  \"type\": \"string\"\n                },\n                \"value\": {\n                  \"description\": \"The value you assign to the custom deny parameter. For available values, see [Deny name values](https://techdocs.akamai.com/application-security/reference/deny-name-values).\",\n                  \"type\": \"string\"\n                }\n              },\n              \"required\": [\n                \"name\",\n                \"value\"\n            \
  \  ],\n              \"type\": \"object\"\n            },\n            \"type\": \"array\"\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"parameters\"\n        ],\n        \"type\": \"object\",\n        \"x-akamai\": {\n          \"file-path\": \"schemas/custom-deny.yaml\"\n        }\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-custom-denies-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: custom-denies
---
