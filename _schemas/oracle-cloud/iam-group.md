---
description: An IAM group.
layout: schema
name: Group
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/iam-group-schema.json
slug: iam-group
source_filename: iam-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-group-schema.json\",\n  \"title\": \"Group\",\n  \"description\": \"An IAM group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Administrators\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['CREATING', 'ACTIVE', 'INACTIVE', 'DELETING', 'DELETED']\",\n      \"example\": \"CREATING\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-group-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Group
---
