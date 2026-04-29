---
description: A route table for a VCN.
layout: schema
name: RouteTable
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: vcnId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: routeRules
  type: array
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-route-table-schema.json
slug: networking-route-table
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-route-table-schema.json\",\n  \"title\": \"RouteTable\",\n  \"description\": \"A route table for a VCN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"Default Route Table\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['PROVISIONING', 'AVAILABLE', 'TERMINATING', 'TERMINATED']\",\n      \"example\": \"PROVISIONING\"\n    },\n    \"routeRules\"\
  : {\n      \"type\": \"array\",\n      \"example\": \"[{'destination': '0.0.0.0/0', 'destinationType': 'CIDR_BLOCK', 'networkEntityId': 'ocid1.resource.oc1.iad.abcdefg123456'}]\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-route-table-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: RouteTable
---
