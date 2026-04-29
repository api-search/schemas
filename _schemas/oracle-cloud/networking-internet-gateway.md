---
description: An internet gateway for a VCN.
layout: schema
name: InternetGateway
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
  name: isEnabled
  type: boolean
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-internet-gateway-schema.json
slug: networking-internet-gateway
source_filename: networking-internet-gateway-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-internet-gateway-schema.json\",\n  \"title\": \"InternetGateway\",\n  \"description\": \"An internet gateway for a VCN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-internet-gateway\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['PROVISIONING', 'AVAILABLE',\
  \ 'TERMINATING', 'TERMINATED']\",\n      \"example\": \"PROVISIONING\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-internet-gateway-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: InternetGateway
---
