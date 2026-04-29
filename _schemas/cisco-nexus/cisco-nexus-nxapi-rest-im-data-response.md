---
description: Standard NX-API REST response wrapper
layout: schema
name: ImDataResponse
properties_list:
- description: Total number of managed objects in the response
  name: totalCount
  type: string
- description: Array of managed object results
  name: imdata
  type: array
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
schema_file: json-schema/cisco-nexus-nxapi-rest-im-data-response-schema.json
slug: cisco-nexus-nxapi-rest-im-data-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ImDataResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard NX-API REST response wrapper\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"string\",\n      \"description\": \"Total number of managed objects in the response\"\n    },\n    \"imdata\": {\n      \"type\": \"array\",\n      \"description\": \"Array of managed object results\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/json-schema/cisco-nexus-nxapi-rest-im-data-response-schema.json
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
title: ImDataResponse
---
