---
description: CreatePolicyDetails schema from oracle-cloud-iam-openapi.yaml
layout: schema
name: CreatePolicyDetails
properties_list:
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
  name: statements
  type: array
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/iam-create-policy-details-schema.json
slug: iam-create-policy-details
source_filename: iam-create-policy-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-create-policy-details-schema.json\",\n  \"title\": \"CreatePolicyDetails\",\n  \"description\": \"CreatePolicyDetails schema from oracle-cloud-iam-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"name\",\n    \"description\",\n    \"statements\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"statements\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/iam-create-policy-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreatePolicyDetails
---
