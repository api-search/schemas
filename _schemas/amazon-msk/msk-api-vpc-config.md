---
description: <p>The configuration of the Amazon VPCs for the cluster.</p>
layout: schema
name: VpcConfig
properties_list:
- description: ''
  name: SubnetIds
  type: object
- description: ''
  name: SecurityGroupIds
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-vpc-config-schema.json
slug: msk-api-vpc-config
source_filename: msk-api-vpc-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-vpc-config-schema.json\",\n  \"title\": \"VpcConfig\",\n  \"description\": \"\\n            <p>The configuration of the Amazon VPCs for the cluster.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SubnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subnetIds\"\n          },\n          \"description\": \"\\n            <p>The IDs of the subnets associated with the cluster.</p>\"\n        }\n      ]\n    },\n    \"SecurityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"securityGroupIds\"\n          },\n          \"description\": \"\\n  \
  \          <p>The IDs of the security groups associated with the cluster.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SubnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-vpc-config-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: VpcConfig
---
