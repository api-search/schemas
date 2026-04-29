---
description: Information about an AWS Cloud9 development environment.
layout: schema
name: Environment
properties_list:
- description: The ID of the environment.
  name: id
  type: string
- description: The name of the environment.
  name: name
  type: string
- description: The description for the environment.
  name: description
  type: string
- description: The type of environment.
  name: type
  type: string
- description: The connection type for connecting to the environment.
  name: connectionType
  type: string
- description: The current status of the environment.
  name: status
  type: string
- description: The Amazon Resource Name (ARN) of the environment owner.
  name: ownerArn
  type: string
provider_name: Amazon Cloud9
provider_slug: amazon-cloud9
schema_file: json-schema/cloud9-environment-schema.json
slug: cloud9-environment
source_filename: cloud9-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-environment-schema.json\",\n  \"title\": \"Environment\",\n  \"description\": \"Information about an AWS Cloud9 development environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the environment.\",\n      \"example\": \"abc12345678901234567890\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the environment.\",\n      \"example\": \"my-dev-environment\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description for the environment.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ssh\",\n        \"ec2\"\n      ],\n      \"description\": \"The type of environment.\"\n    },\n    \"connectionType\"\
  : {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONNECT_SSH\",\n        \"CONNECT_SSM\"\n      ],\n      \"description\": \"The connection type for connecting to the environment.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"error\",\n        \"creating\",\n        \"connecting\",\n        \"ready\",\n        \"stopping\",\n        \"stopped\",\n        \"deleting\"\n      ],\n      \"description\": \"The current status of the environment.\"\n    },\n    \"ownerArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the environment owner.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-environment-schema.json
tags:
- AWS
- Cloud9
- IDE
- Development
- Browser-Based
title: Environment
---
