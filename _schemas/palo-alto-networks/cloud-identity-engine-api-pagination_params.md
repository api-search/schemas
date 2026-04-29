---
description: Optional pagination parameters.
layout: schema
name: pagination_params
properties_list:
- description: Page number to retrieve (starting from page 1).
  name: pageNum
  type: integer
- description: Number of records per page (max is 1000 per page).
  name: pageSz
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-pagination_params-schema.json
slug: cloud-identity-engine-api-pagination_params
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"pagination_params\",\n  \"description\": \"Optional pagination parameters.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-pagination_params-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pageNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Page number to retrieve (starting from page 1).\",\n      \"example\": 1\n    },\n    \"pageSz\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records per page (max is 1000 per page).\",\n      \"example\": 500\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-pagination_params-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: pagination_params
---
