---
description: JSON Schema for Lambda Cloud API resources.
layout: schema
name: Lambda Cloud API Resources
properties_list: []
provider_name: Lambda
provider_slug: lambda
schema_file: json-schema/lambda-cloud-api-schema.json
slug: lambda-cloud-api
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/lambda/json-schema/lambda-cloud-api-schema.json\",\n  \"title\": \"Lambda Cloud API Resources\",\n  \"description\": \"JSON Schema for Lambda Cloud API resources.\",\n  \"definitions\": {\n    \"Instance\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the instance.\"\n        },\n        \"name\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"User-provided name for the instance.\"\n        },\n        \"ip\": {\n          \"type\": \"string\",\n          \"description\": \"IPv4 address of the instance.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"booting\", \"unhealthy\", \"terminated\"]\n        },\n        \"ssh_key_names\": {\n          \"type\": \"array\"\
  ,\n          \"items\": { \"type\": \"string\" }\n        },\n        \"file_system_names\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" }\n        },\n        \"region\": { \"$ref\": \"#/definitions/Region\" },\n        \"instance_type\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"description\": { \"type\": \"string\" }\n          }\n        },\n        \"hostname\": { \"type\": \"string\" },\n        \"jupyter_token\": { \"type\": \"string\" },\n        \"jupyter_url\": { \"type\": \"string\" }\n      },\n      \"required\": [\"id\", \"status\"]\n    },\n    \"Region\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" }\n      },\n      \"required\": [\"name\"]\n    },\n    \"InstanceType\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"instance_type\"\
  : {\n          \"type\": \"object\",\n          \"properties\": {\n            \"name\": { \"type\": \"string\" },\n            \"description\": { \"type\": \"string\" },\n            \"price_cents_per_hour\": { \"type\": \"integer\" },\n            \"specs\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"vcpus\": { \"type\": \"integer\" },\n                \"memory_gib\": { \"type\": \"integer\" },\n                \"storage_gib\": { \"type\": \"integer\" }\n              }\n            }\n          }\n        },\n        \"regions_with_capacity_available\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/definitions/Region\" }\n        }\n      }\n    },\n    \"SshKey\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"public_key\": { \"type\": \"string\" },\n        \"private_key\": { \"type\": [\"string\", \"\
  null\"] }\n      },\n      \"required\": [\"id\", \"name\"]\n    },\n    \"FileSystem\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" },\n        \"created\": { \"type\": \"string\", \"format\": \"date-time\" },\n        \"mount_point\": { \"type\": \"string\" },\n        \"region\": { \"$ref\": \"#/definitions/Region\" }\n      },\n      \"required\": [\"id\", \"name\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/lambda/refs/heads/main/json-schema/lambda-cloud-api-schema.json
tags:
- Artificial Intelligence
- Cloud Computing
- Compute
- Deep Learning
- GPU
- Machine Learning
title: Lambda Cloud API Resources
---
