---
description: Retrieve all users in a domain.
layout: schema
name: list_all_users_in_domain
properties_list:
- description: User attributes included as part of the response.
  name: attrs
  type: array
- description: ''
  name: useNormalizedAttrs
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-list_all_users_in_domain-schema.json
slug: cloud-identity-engine-api-list_all_users_in_domain
source_filename: cloud-identity-engine-api-list_all_users_in_domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"list_all_users_in_domain\",\n  \"description\": \"Retrieve all users in a domain.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_all_users_in_domain-schema.json\",\n  \"properties\": {\n    \"attrs\": {\n      \"type\": \"array\",\n      \"description\": \"User attributes included as part of the response.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"Common-Name\",\n        \"Mail\",\n        \"Unique Identifier\",\n        \"Manager\",\n        \"User Principal Name\",\n        \"Name\",\n        \"Distinguished Name\",\n        \"SAM Account Name\"\n      ]\n    },\n    \"useNormalizedAttrs\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"True\",\n        \"False\"\n      ],\n      \"example\": \"True\"\n    }\n  },\n  \"allOf\":\
  \ [\n    {\n      \"type\": \"object\",\n      \"description\": \"Domain name for a specific directory.\",\n      \"required\": [\n        \"domain\"\n      ],\n      \"properties\": {\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"Domain name of the target directory.\",\n          \"example\": \"paloaltonetworks.com\"\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"description\": \"Optional pagination parameters.\",\n      \"properties\": {\n        \"pageNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Page number to retrieve (starting from page 1).\",\n          \"example\": 1\n        },\n        \"pageSz\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of records per page (max is 1000 per page).\",\n          \"example\": 500\n        }\n      }\n    }\n  ],\n  \"type\": \"object\"\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-list_all_users_in_domain-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: list_all_users_in_domain
---
