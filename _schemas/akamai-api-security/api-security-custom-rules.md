---
description: Describes the custom rule's basic information.
layout: schema
name: custom-rules
properties_list:
- description: Describes basic information about a custom rule, such as activation status or time the rule is active.
  name: customRules
  type: array
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-custom-rules-schema.json
slug: api-security-custom-rules
source_filename: api-security-custom-rules-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-custom-rules-schema.json\",\n  \"title\": \"custom-rules\",\n  \"description\": \"Describes the custom rule's basic information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customRules\": {\n      \"description\": \"Describes basic information about a custom rule, such as activation status or time the rule is active.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"effectiveTimePeriod\": {\n            \"additionalProperties\": false,\n            \"description\": \"The time period during which the custom rule is active.\",\n            \"properties\": {\n              \"endDate\": {\n                \"description\": \"An ISO 8601 timestamp that sets when the rule expires or deactivates.\",\n                \"type\": \"\
  string\"\n              },\n              \"startDate\": {\n                \"description\": \"An ISO 8601 timestamp that sets when the rule activates.\",\n                \"format\": \"date-time\",\n                \"type\": \"string\"\n              },\n              \"status\": {\n                \"description\": \"The current status of the rule based on its `startDate` and `endDate`. By default, rules are active for 30 days. When `ACTIVE`, the rule triggers when conditions are met. When `INACTIVE`, the rule doesn't trigger. When `EXPIRING`, the rule still triggers because it's still active until its specified expiration date. When the rule's status is `EXPIRED`, the rule is inactive and doesn't trigger. If your rule expires and you want to use it again, make a PUT request to [Modify a custom rule](https://techdocs.akamai.com/application-security/reference/put-config-custom-rule) with the new dates you'd like the rule to be active.\",\n                \"enum\": [\n                 \
  \ \"active\",\n                  \"inactive\",\n                  \"expiring\",\n                  \"expired\"\n                ],\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"endDate\",\n              \"startDate\"\n            ],\n            \"type\": \"object\"\n          },\n          \"id\": {\n            \"description\": \"Uniquely identifies the custom rule.\",\n            \"type\": \"integer\"\n          },\n          \"link\": {\n            \"description\": \"The link to the full custom rule definition. This member is only available when you run the [List custom rules](https://techdocs.akamai.com/application-security/reference/get-configs-custom-rules) operation.\",\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"The name you assign to the custom rule.\",\n            \"type\": \"string\"\n          },\n          \"samplingRate\": {\n            \"\
  description\": \"The portion of traffic to sample, expressed as a percent.\",\n            \"maximum\": 100,\n            \"minimum\": 0,\n            \"type\": \"integer\"\n          },\n          \"status\": {\n            \"description\": \"The custom rule deployment status. Either `activated` if a rule is enabled in at least one security policy within a security configuration currently active in production, `published` if a rule is associated with at least one security policy in an inactive security configuration, or `unused` if a rule exists as a shared resource, but isn't associated with any security policy. This member is only available when you run the [List custom rules](https://techdocs.akamai.com/application-security/reference/get-configs-custom-rules) operation.\",\n            \"enum\": [\n              \"activated\",\n              \"published\",\n              \"unused\"\n            ],\n            \"type\": \"string\"\n          },\n          \"version\": {\n         \
  \   \"description\": \"The custom rule version.\",\n            \"type\": \"integer\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"link\",\n          \"name\",\n          \"status\",\n          \"version\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"required\": [\n    \"customRules\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-custom-rules-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: custom-rules
---
