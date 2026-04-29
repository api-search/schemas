---
description: An Amazon Lightsail virtual server instance.
layout: schema
name: Instance
properties_list:
- description: The name the user gave the instance.
  name: name
  type: string
- description: The Amazon Resource Name (ARN) of the instance.
  name: arn
  type: string
- description: The blueprint ID of the instance.
  name: blueprintId
  type: string
- description: The bundle for the instance.
  name: bundleId
  type: string
- description: The public IP address of the instance.
  name: publicIpAddress
  type: string
- description: The private IP address of the instance.
  name: privateIpAddress
  type: string
- description: The timestamp when the instance was created.
  name: createdAt
  type: string
provider_name: Amazon Lightsail
provider_slug: amazon-lightsail
schema_file: json-schema/amazon-lightsail-instance-schema.json
slug: amazon-lightsail-instance
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lightsail/refs/heads/main/json-schema/amazon-lightsail-instance-schema.json\",\n  \"title\": \"Instance\",\n  \"description\": \"An Amazon Lightsail virtual server instance.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name the user gave the instance.\",\n      \"example\": \"my-wordpress-site\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the instance.\"\n    },\n    \"blueprintId\": {\n      \"type\": \"string\",\n      \"description\": \"The blueprint ID of the instance.\",\n      \"example\": \"wordpress_5_7\"\n    },\n    \"bundleId\": {\n      \"type\": \"string\",\n      \"description\": \"The bundle for the instance.\",\n      \"example\": \"micro_2_0\"\n    },\n    \"publicIpAddress\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The public IP address of the instance.\",\n      \"example\": \"54.123.45.67\"\n    },\n    \"privateIpAddress\": {\n      \"type\": \"string\",\n      \"description\": \"The private IP address of the instance.\",\n      \"example\": \"172.26.0.5\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the instance was created.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lightsail/refs/heads/main/json-schema/amazon-lightsail-instance-schema.json
tags: []
title: Instance
---
