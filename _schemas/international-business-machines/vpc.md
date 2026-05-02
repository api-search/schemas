---
description: An IBM Cloud Virtual Private Cloud (VPC) resource.
layout: schema
name: Virtual Private Cloud
properties_list:
- description: The unique identifier of the VPC.
  name: id
  type: string
- description: The name of the VPC.
  name: name
  type: string
- description: The status of the VPC.
  name: status
  type: string
- description: The Cloud Resource Name (CRN) of the VPC.
  name: crn
  type: string
- description: Whether classic access is enabled.
  name: classic_access
  type: boolean
- description: The date and time the VPC was created.
  name: created_at
  type: string
- description: ''
  name: default_security_group
  type: object
- description: ''
  name: resource_group
  type: object
provider_name: International Business Machines
provider_slug: international-business-machines
schema_file: json-schema/vpc.json
slug: vpc
source_filename: vpc.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"vpc.json\",\n  \"title\": \"Virtual Private Cloud\",\n  \"description\": \"An IBM Cloud Virtual Private Cloud (VPC) resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the VPC.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the VPC.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the VPC.\",\n      \"enum\": [\"available\", \"deleting\", \"failed\", \"pending\"]\n    },\n    \"crn\": {\n      \"type\": \"string\",\n      \"description\": \"The Cloud Resource Name (CRN) of the VPC.\"\n    },\n    \"classic_access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether classic access is enabled.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The date and time the VPC was created.\"\n    },\n    \"default_security_group\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"resource_group\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    }\n  },\n  \"required\": [\"id\", \"name\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/international-business-machines/refs/heads/main/json-schema/vpc.json
tags:
- Artificial Intelligence
- Cloud
- Enterprise
- IBM
title: Virtual Private Cloud
---
