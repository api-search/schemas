---
description: A set of firewall rules for a VCN subnet.
layout: schema
name: SecurityList
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
  name: ingressSecurityRules
  type: array
- description: ''
  name: egressSecurityRules
  type: array
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-security-list-schema.json
slug: networking-security-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-security-list-schema.json\",\n  \"title\": \"SecurityList\",\n  \"description\": \"A set of firewall rules for a VCN subnet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"Default Security List\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['PROVISIONING', 'AVAILABLE', 'TERMINATING', 'TERMINATED']\",\n      \"example\": \"PROVISIONING\"\
  \n    },\n    \"ingressSecurityRules\": {\n      \"type\": \"array\",\n      \"example\": \"[{'protocol': '6', 'source': '0.0.0.0/0', 'isStateless': True}]\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"egressSecurityRules\": {\n      \"type\": \"array\",\n      \"example\": \"[{'protocol': 'example-value', 'destination': 'example-value', 'isStateless': True}]\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-security-list-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: SecurityList
---
