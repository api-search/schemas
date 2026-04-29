---
description: A virtual cloud network in Oracle Cloud Infrastructure.
layout: schema
name: Vcn
properties_list:
- description: The OCID of the VCN.
  name: id
  type: string
- description: The OCID of the compartment.
  name: compartmentId
  type: string
- description: A user-friendly name.
  name: displayName
  type: string
- description: The CIDR block of the VCN.
  name: cidrBlock
  type: string
- description: List of CIDR blocks.
  name: cidrBlocks
  type: array
- description: The OCID of the default DHCP options.
  name: defaultDhcpOptionsId
  type: string
- description: The OCID of the default route table.
  name: defaultRouteTableId
  type: string
- description: The OCID of the default security list.
  name: defaultSecurityListId
  type: string
- description: The DNS label for the VCN.
  name: dnsLabel
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
- description: ''
  name: freeformTags
  type: object
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/networking-vcn-schema.json
slug: networking-vcn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-vcn-schema.json\",\n  \"title\": \"Vcn\",\n  \"description\": \"A virtual cloud network in Oracle Cloud Infrastructure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the VCN.\",\n      \"example\": \"ocid1.vcn.oc1.iad.abcdefg123456\"\n    },\n    \"compartmentId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the compartment.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A user-friendly name.\",\n      \"example\": \"my-vcn\"\n    },\n    \"cidrBlock\": {\n      \"type\": \"string\",\n      \"description\": \"The CIDR block of the VCN.\",\n      \"example\": \"10.0.0.0/16\"\n    },\n\
  \    \"cidrBlocks\": {\n      \"type\": \"array\",\n      \"description\": \"List of CIDR blocks.\",\n      \"example\": \"['10.0.0.0/16']\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"defaultDhcpOptionsId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the default DHCP options.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"defaultRouteTableId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the default route table.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"defaultSecurityListId\": {\n      \"type\": \"string\",\n      \"description\": \"The OCID of the default security list.\",\n      \"example\": \"ocid1.resource.oc1.iad.abcdefg123456\"\n    },\n    \"dnsLabel\": {\n      \"type\": \"string\",\n      \"description\": \"The DNS label for the VCN.\",\n      \"example\": \"myvcn\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": \"['PROVISIONING', 'AVAILABLE', 'TERMINATING', 'TERMINATED']\",\n      \"example\": \"PROVISIONING\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"freeformTags\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key1\": \"value1\"\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/networking-vcn-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: Vcn
---
