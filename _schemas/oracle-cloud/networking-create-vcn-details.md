---
description: CreateVcnDetails schema from oracle-cloud-networking-openapi.yaml
layout: schema
name: CreateVcnDetails
properties_list:
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: List of CIDR blocks for the VCN.
  name: cidrBlocks
  type: array
- description: A user-friendly name.
  name: displayName
  type: string
- description: DNS label for the VCN.
  name: dnsLabel
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-create-vcn-details-schema.json
slug: networking-create-vcn-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-create-vcn-details-schema.json\",\n  \"title\": \"CreateVcnDetails\",\n  \"description\": \"CreateVcnDetails schema from oracle-cloud-networking-openapi.yaml\",\n  \"type\": \"object\",\n  \"required\": [\n    \"compartmentId\",\n    \"cidrBlocks\"\n  ],\n  \"properties\": {\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"cidrBlocks\": {\n      \"type\": \"array\",\n      \"description\": \"List of CIDR blocks for the VCN.\",\n      \"example\": \"['10.0.0.0/16']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\",\n      \"example\": \"\
  my-vcn\"\n    },\n    \"dnsLabel\": {\n      \"type\": \"string\",\n      \"description\": \"DNS label for the VCN.\",\n      \"example\": \"myvcn\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-create-vcn-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: CreateVcnDetails
---
