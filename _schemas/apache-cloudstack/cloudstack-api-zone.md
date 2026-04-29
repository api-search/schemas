---
description: A CloudStack availability zone grouping compute, network, and storage resources.
layout: schema
name: Zone
properties_list:
- description: UUID of the zone.
  name: id
  type: string
- description: Name of the zone.
  name: name
  type: string
- description: Network type of the zone (Basic or Advanced).
  name: networktype
  type: string
- description: Allocation state of the zone (Enabled or Disabled).
  name: allocationstate
  type: string
- description: Whether security groups are enabled in the zone.
  name: securitygroupsenabled
  type: boolean
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-zone-schema.json
slug: cloudstack-api-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-zone-schema.json\",\n  \"title\": \"Zone\",\n  \"description\": \"A CloudStack availability zone grouping compute, network, and storage resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"UUID of the zone.\", \"example\": \"zone-uuid-abcd\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Name of the zone.\", \"example\": \"us-east-1\" },\n    \"networktype\": { \"type\": \"string\", \"description\": \"Network type of the zone (Basic or Advanced).\", \"enum\": [\"Basic\", \"Advanced\"], \"example\": \"Advanced\" },\n    \"allocationstate\": { \"type\": \"string\", \"description\": \"Allocation state of the zone (Enabled or Disabled).\", \"example\": \"Enabled\" },\n    \"securitygroupsenabled\": { \"type\": \"\
  boolean\", \"description\": \"Whether security groups are enabled in the zone.\", \"example\": false }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cloudstack/refs/heads/main/json-schema/cloudstack-api-zone-schema.json
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: Zone
---
