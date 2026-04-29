---
description: CreateInternetGatewayDetails schema from oracle-cloud-networking-openapi.yaml
layout: schema
name: CreateInternetGatewayDetails
properties_list:
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: vcnId
  type: string
- description: ''
  name: isEnabled
  type: boolean
- description: ''
  name: displayName
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-create-internet-gateway-details-schema.json
slug: networking-create-internet-gateway-details
source_filename: networking-create-internet-gateway-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-create-internet-gateway-details-schema.json\",\n  \"title\": \"CreateInternetGatewayDetails\",\n  \"description\": \"CreateInternetGatewayDetails schema from oracle-cloud-networking-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"vcnId\",\n    \"isEnabled\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"isEnabled\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"default\": true\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"my-resource\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-create-internet-gateway-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateInternetGatewayDetails
---
