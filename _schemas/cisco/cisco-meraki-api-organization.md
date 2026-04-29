---
description: A Meraki organization.
layout: schema
name: Organization
properties_list:
- description: Organization ID.
  name: id
  type: string
- description: Organization name.
  name: name
  type: string
- description: Organization URL in the Meraki dashboard.
  name: url
  type: string
provider_name: Cisco
provider_slug: cisco
schema_file: json-schema/cisco-meraki-api-organization-schema.json
slug: cisco-meraki-api-organization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/json-schema/cisco-meraki-api-organization-schema.json\",\n  \"title\": \"Organization\",\n  \"description\": \"A Meraki organization.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Organization ID.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Organization name.\" },\n    \"url\": { \"type\": \"string\", \"description\": \"Organization URL in the Meraki dashboard.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/json-schema/cisco-meraki-api-organization-schema.json
tags:
- Collaboration
- Enterprise
- Networking
- Security
- SD-WAN
title: Organization
---
