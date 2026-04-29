---
description: Contains Security Information Event Management (SIEM) integration settings.
layout: schema
name: siem-settings
properties_list:
- description: Whether you enabled SIEM for all the security policies in the configuration version.
  name: enableForAllPolicies
  type: boolean
- description: Whether you enabled SIEM in a security configuration version.
  name: enableSiem
  type: boolean
- description: __Deprecated__ Whether you enabled SIEM for the Bot Manager events. Use `exceptions` parameter instead to set botman siem events exception.
  name: enabledBotmanSiemEvents
  type: boolean
- description: Describes all attack type exceptions that will be ignored in siem events.
  name: exceptions
  type: array
- description: The list of security policy identifiers for which to enable the SIEM integration.
  name: firewallPolicyIds
  type: array
- description: Uniquely identifies the SIEM settings.
  name: siemDefinitionId
  type: integer
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-siem-settings-schema.json
slug: api-security-siem-settings
source_filename: api-security-siem-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-siem-settings-schema.json\",\n  \"title\": \"siem-settings\",\n  \"description\": \"Contains Security Information Event Management (SIEM) integration settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enableForAllPolicies\": {\n      \"description\": \"Whether you enabled SIEM for all the security policies in the configuration version.\",\n      \"type\": \"boolean\"\n    },\n    \"enableSiem\": {\n      \"description\": \"Whether you enabled SIEM in a security configuration version.\",\n      \"type\": \"boolean\"\n    },\n    \"enabledBotmanSiemEvents\": {\n      \"description\": \"__Deprecated__ Whether you enabled SIEM for the Bot Manager events. Use `exceptions` parameter instead to set botman siem events exception. \",\n      \"type\": \"boolean\",\n      \"x-akamai\"\
  : {\n        \"status\": \"DEPRECATED\"\n      }\n    },\n    \"exceptions\": {\n      \"description\": \"Describes all attack type exceptions that will be ignored in siem events.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"actionTypes\": {\n            \"description\": \"Describes actions to be excluded for a particular attack type. A `*` value means all actions.\",\n            \"items\": {\n              \"enum\": [\n                \"*\",\n                \"alert\",\n                \"deny\",\n                \"all_custom\",\n                \"abort\",\n                \"allow\",\n                \"delay\",\n                \"ignore\",\n                \"monitor\",\n                \"slow\",\n                \"tarpit\"\n              ],\n              \"type\": \"string\"\n            },\n            \"type\": \"array\"\n          },\n          \"protection\": {\n            \"description\": \"Attack type to be added as an\
  \ exception.\",\n            \"enum\": [\n              \"ipgeo\",\n              \"rate\",\n              \"urlProtection\",\n              \"slowpost\",\n              \"customrules\",\n              \"waf\",\n              \"apirequestconstraints\",\n              \"clientrep\",\n              \"malwareprotection\",\n              \"botmanagement\",\n              \"aprProtection\"\n            ],\n            \"type\": \"string\"\n          }\n        },\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"firewallPolicyIds\": {\n      \"description\": \"The list of security policy identifiers for which to enable the SIEM integration.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"siemDefinitionId\": {\n      \"description\": \"Uniquely identifies the SIEM settings.\",\n      \"type\": \"integer\"\n    }\n  },\n  \"required\": [\n    \"enableSiem\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-siem-settings-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: siem-settings
---
