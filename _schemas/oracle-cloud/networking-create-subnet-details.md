---
description: CreateSubnetDetails schema from oracle-cloud-networking-openapi.yaml
layout: schema
name: CreateSubnetDetails
properties_list:
- description: ''
  name: compartmentId
  type: string
- description: ''
  name: vcnId
  type: string
- description: ''
  name: cidrBlock
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: dnsLabel
  type: string
- description: ''
  name: prohibitPublicIpOnVnic
  type: boolean
- description: ''
  name: routeTableId
  type: string
- description: ''
  name: securityListIds
  type: array
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-create-subnet-details-schema.json
slug: networking-create-subnet-details
source_filename: networking-create-subnet-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-create-subnet-details-schema.json\",\n  \"title\": \"CreateSubnetDetails\",\n  \"description\": \"CreateSubnetDetails schema from oracle-cloud-networking-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"vcnId\",\n    \"cidrBlock\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"cidrBlock\": {\n      \"type\": \"string\",\n      \"example\": \"10.0.0.0/24\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"public-subnet-1\"\n    },\n    \"dnsLabel\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"myresource\"\n    },\n    \"prohibitPublicIpOnVnic\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"default\": false\n    },\n    \"routeTableId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"securityListIds\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-create-subnet-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateSubnetDetails
---
