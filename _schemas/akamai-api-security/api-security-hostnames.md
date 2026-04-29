---
description: Contains a list of selected hostnames for the specified configuration version.
layout: schema
name: hostnames
properties_list:
- description: The list of hostnames for a configuration version.
  name: hostnameList
  type: array
- description: The type of update you want to make to the evaluation hostname list. Use `append` to add additional hostnames, `remove` to delete the hostnames from the list, or `replace` to replace the existing list
  name: mode
  type: string
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-hostnames-schema.json
slug: api-security-hostnames
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostnames-schema.json\",\n  \"title\": \"hostnames\",\n  \"description\": \"Contains a list of selected hostnames for the specified configuration version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"hostnameList\": {\n      \"description\": \"The list of hostnames for a configuration version.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"hostname\": {\n            \"description\": \"The hostname on which to match the request.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"hostname\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"mode\": {\n      \"description\": \"The type of update you want to make to the evaluation\
  \ hostname list. Use `append` to add additional hostnames, `remove` to delete the hostnames from the list, or `replace` to replace the existing list with the hostnames you pass in your request.\",\n      \"enum\": [\n        \"append\",\n        \"remove\",\n        \"replace\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"hostnameList\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostnames-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: hostnames
---
