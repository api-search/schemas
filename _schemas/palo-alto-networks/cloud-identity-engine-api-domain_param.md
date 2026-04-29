---
description: Domain name for a specific directory.
layout: schema
name: domain_param
properties_list:
- description: Domain name of the target directory.
  name: domain
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cloud-identity-engine-api-domain_param-schema.json
slug: cloud-identity-engine-api-domain_param
source_filename: cloud-identity-engine-api-domain_param-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"domain_param\",\n  \"description\": \"Domain name for a specific directory.\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-domain_param-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Domain name of the target directory.\",\n      \"example\": \"paloaltonetworks.com\"\n    }\n  },\n  \"required\": [\n    \"domain\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cloud-identity-engine-api-domain_param-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: domain_param
---
