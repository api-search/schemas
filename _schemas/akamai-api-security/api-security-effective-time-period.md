---
description: The time period during which the custom rule is active.
layout: schema
name: effectiveTimePeriod
properties_list:
- description: An ISO 8601 timestamp that sets when the rule expires or deactivates.
  name: endDate
  type: string
- description: An ISO 8601 timestamp that sets when the rule activates.
  name: startDate
  type: string
- description: The current status of the rule based on its `startDate` and `endDate`. By default, rules are active for 30 days. When `ACTIVE`, the rule triggers when conditions are met. When `INACTIVE`, the rule doe
  name: status
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-effective-time-period-schema.json
slug: api-security-effective-time-period
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-effective-time-period-schema.json\",\n  \"title\": \"effectiveTimePeriod\",\n  \"description\": \"The time period during which the custom rule is active.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endDate\": {\n      \"description\": \"An ISO 8601 timestamp that sets when the rule expires or deactivates.\",\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"description\": \"An ISO 8601 timestamp that sets when the rule activates.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The current status of the rule based on its `startDate` and `endDate`. By default, rules are active for 30 days. When `ACTIVE`, the rule triggers when conditions are met. When `INACTIVE`, the rule doesn't trigger. When\
  \ `EXPIRING`, the rule still triggers because it's still active until its specified expiration date. When the rule's status is `EXPIRED`, the rule is inactive and doesn't trigger. If your rule expires and you want to use it again, make a PUT request to [Modify a custom rule](https://techdocs.akamai.com/application-security/reference/put-config-custom-rule) with the new dates you'd like the rule to be active.\",\n      \"enum\": [\n        \"active\",\n        \"inactive\",\n        \"expiring\",\n        \"expired\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"endDate\",\n    \"startDate\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-effective-time-period-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: effectiveTimePeriod
---
