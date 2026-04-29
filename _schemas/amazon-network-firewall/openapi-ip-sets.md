---
description: IPSets schema from Amazon Network Firewall
layout: schema
name: IPSets
properties_list: []
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-ip-sets-schema.json
slug: openapi-ip-sets
source_filename: openapi-ip-sets-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-ip-sets-schema.json\",\n  \"title\": \"IPSets\",\n  \"description\": \"IPSets schema from Amazon Network Firewall\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/IPSet\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-ip-sets-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: IPSets
---
