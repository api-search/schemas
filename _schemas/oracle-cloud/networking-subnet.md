---
description: A subnet in a virtual cloud network.
layout: schema
name: Subnet
properties_list:
- description: The OCID of the subnet.
  name: id
  type: string
- description: ''
  name: compartmentId
  type: string
- description: The OCID of the VCN.
  name: vcnId
  type: string
- description: ''
  name: displayName
  type: string
- description: The CIDR block of the subnet.
  name: cidrBlock
  type: string
- description: The availability domain.
  name: availabilityDomain
  type: string
- description: ''
  name: dnsLabel
  type: string
- description: Whether VNICs can have public IPs.
  name: prohibitPublicIpOnVnic
  type: boolean
- description: ''
  name: routeTableId
  type: string
- description: ''
  name: securityListIds
  type: array
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-subnet-schema.json
slug: networking-subnet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-subnet-schema.json\",\n  \"title\": \"Subnet\",\n  \"description\": \"A subnet in a virtual cloud network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the subnet.\",\n      \"example\": \"ocid1.subnet.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"vcnId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the VCN.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"example\": \"public-subnet-1\"\n    },\n    \"cidrBlock\": {\n      \"type\": \"string\",\n      \"description\": \"The CIDR block of\
  \ the subnet.\",\n      \"example\": \"10.0.0.0/24\"\n    },\n    \"availabilityDomain\": {\n      \"type\": \"string\",\n      \"description\": \"The availability domain.\",\n      \"example\": \"Uocm:US-ASHBURN-AD-1\"\n    },\n    \"dnsLabel\": {\n      \"type\": \"string\",\n      \"example\": \"myresource\"\n    },\n    \"prohibitPublicIpOnVnic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether VNICs can have public IPs.\",\n      \"example\": true\n    },\n    \"routeTableId\": {\n      \"type\": \"string\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"securityListIds\": {\n      \"type\": \"array\",\n      \"example\": \"['example-value']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\",\n      \"enum\": \"['PROVISIONING', 'AVAILABLE', 'TERMINATING', 'TERMINATED']\",\n      \"example\": \"PROVISIONING\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-subnet-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Subnet
---
