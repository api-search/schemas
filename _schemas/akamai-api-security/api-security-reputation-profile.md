---
description: Contains details about a reputation profile.
layout: schema
name: reputation-profile
properties_list:
- description: Contains information about the criteria that trigger the reputation profile.
  name: condition
  type: object
- description: Identifies the reputation category. Web scrapers (`WEBSCRP`) crawl sites and collect data like hotel rates, product prices, store locations, and more. DoS attackers (`DOSATCK`) are web clients or botn
  name: context
  type: string
- description: __Read-only__ Describes the reputation category.
  name: contextReadable
  type: string
- description: Describes the reputation profile.
  name: description
  type: string
- description: __Read-only__ Whether you enabled the reputation profile.
  name: enabled
  type: boolean
- description: __Read-only__ Uniquely identifies the reputation profile.
  name: id
  type: integer
- description: The name you assigned to the reputation profile.
  name: name
  type: string
- description: Identifies the IP sharing. Either `NON_SHARED`, `SHARED_ONLY`, `BOTH`.
  name: sharedIpHandling
  type: string
- description: The threshold when the profile to triggers.
  name: threshold
  type: number
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-reputation-profile-schema.json
slug: api-security-reputation-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-reputation-profile-schema.json\",\n  \"title\": \"reputation-profile\",\n  \"description\": \"Contains details about a reputation profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"condition\": {\n      \"additionalProperties\": false,\n      \"description\": \"Contains information about the criteria that trigger the reputation profile.\",\n      \"properties\": {\n        \"atomicConditions\": {\n          \"description\": \"The conditions that trigger the reputation profile.\",\n          \"items\": {\n            \"additionalProperties\": false,\n            \"properties\": {\n              \"positiveMatch\": {\n                \"description\": \"Whether the condition should trigger on a match (`true`) or a lack of match (`false`).\",\n                \"type\": \"boolean\"\
  \n              },\n              \"type\": {\n                \"description\": \"The condition type. For available values, see [Condition Values](https://techdocs.akamai.com/application-security/reference/condition-values).\",\n                \"enum\": [\n                  \"NetworkListCondition\",\n                  \"AsNumberCondition\",\n                  \"IpAddressCondition\",\n                  \"RequestCookieCondition\",\n                  \"RequestHeaderCondition\",\n                  \"HostCondition\",\n                  \"UrlPatternCondition\"\n                ],\n                \"type\": \"string\"\n              },\n              \"value\": {\n                \"description\": \"The list of values that trigger the condition.\",\n                \"items\": {\n                  \"type\": \"string\"\n                },\n                \"minItems\": 1,\n                \"type\": \"array\",\n                \"uniqueItems\": true\n              },\n              \"valueCase\"\
  : {\n                \"default\": false,\n                \"description\": \"Whether to consider the character case when comparing the value string with the request value. The default is `false`, meaning that a value such as `url` would match a string `UrL` in the request.\",\n                \"type\": \"boolean\"\n              },\n              \"valueWildcard\": {\n                \"default\": true,\n                \"description\": \"Whether to treat the asterisk (`*`) and question mark (`?`) as wildcards when comparing the value string with the request value. Note that setting this to `false` isn't supported by the host condition, and means that the value string must match exactly.\",\n                \"type\": \"boolean\"\n              }\n            },\n            \"type\": \"object\"\n          },\n          \"type\": \"array\"\n        },\n        \"positiveMatch\": {\n          \"description\": \"Whether the condition should trigger on a match (`true`) or a lack of match (`false`).\"\
  ,\n          \"type\": \"boolean\"\n        }\n      },\n      \"type\": \"object\"\n    },\n    \"context\": {\n      \"description\": \"Identifies the reputation category. Web scrapers (`WEBSCRP`) crawl sites and collect data like hotel rates, product prices, store locations, and more. DoS attackers (`DOSATCK`) are web clients or botnets that use automated tools to launch volumetric Denial of Service (DoS) attacks. Web attackers (`WEBATCK`) target websites and web apps with techniques like SQL injection, remote file inclusion, or cross-site scripting. Scanning tools (`SCANTL`) probe web apps for vulnerabilities during an attack's reconnaissance phase.\",\n      \"enum\": [\n        \"WEBSCRP\",\n        \"DOSATCK\",\n        \"WEBATCK\",\n        \"SCANTL\"\n      ],\n      \"type\": \"string\"\n    },\n    \"contextReadable\": {\n      \"description\": \"__Read-only__ Describes the reputation category.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"description\"\
  : {\n      \"description\": \"Describes the reputation profile.\",\n      \"type\": \"string\"\n    },\n    \"enabled\": {\n      \"description\": \"__Read-only__ Whether you enabled the reputation profile.\",\n      \"readOnly\": true,\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"description\": \"__Read-only__ Uniquely identifies the reputation profile.\",\n      \"readOnly\": true,\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"description\": \"The name you assigned to the reputation profile.\",\n      \"type\": \"string\"\n    },\n    \"sharedIpHandling\": {\n      \"description\": \"Identifies the IP sharing. Either `NON_SHARED`, `SHARED_ONLY`, `BOTH`.\",\n      \"enum\": [\n        \"NON_SHARED\",\n        \"SHARED_ONLY\",\n        \"BOTH\"\n      ],\n      \"type\": \"string\"\n    },\n    \"threshold\": {\n      \"description\": \"The threshold when the profile to triggers.\",\n      \"type\": \"number\"\n    }\n  },\n  \"required\": [\n    \"name\"\
  ,\n    \"context\",\n    \"threshold\",\n    \"sharedIpHandling\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-reputation-profile-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: reputation-profile
---
