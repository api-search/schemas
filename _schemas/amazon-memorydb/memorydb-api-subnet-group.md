---
description: 'Represents the output of one of the following operations: CreateSubnetGroup / DescribeSubnetGroups.'
layout: schema
name: SubnetGroup
properties_list:
- description: The ARN of the subnet group.
  name: ARN
  type: string
- description: A description of the subnet group.
  name: Description
  type: string
- description: The name of the subnet group.
  name: Name
  type: string
- description: The Amazon Virtual Private Cloud identifier (VPC ID) of the subnet group.
  name: VpcId
  type: string
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-subnet-group-schema.json
slug: memorydb-api-subnet-group
source_filename: memorydb-api-subnet-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-subnet-group-schema.json\",\n  \"title\": \"SubnetGroup\",\n  \"description\": \"Represents the output of one of the following operations: CreateSubnetGroup / DescribeSubnetGroups.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ARN\": {\n      \"description\": \"The ARN of the subnet group.\",\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"description\": \"A description of the subnet group.\",\n      \"type\": \"string\"\n    },\n    \"Name\": {\n      \"description\": \"The name of the subnet group.\",\n      \"type\": \"string\"\n    },\n    \"VpcId\": {\n      \"description\": \"The Amazon Virtual Private Cloud identifier (VPC ID) of the subnet group.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-subnet-group-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: SubnetGroup
---
