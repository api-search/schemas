---
description: Request body for creating an EC2-based Cloud9 environment.
layout: schema
name: CreateEnvironmentEC2Request
properties_list:
- description: The name of the environment.
  name: name
  type: string
- description: The description of the environment.
  name: description
  type: string
- description: The type of instance to connect to the environment.
  name: instanceType
  type: string
- description: The connection type to use for connecting to the environment.
  name: connectionType
  type: string
- description: The number of minutes until the running instance is shut down after the environment has last been used.
  name: automaticStopTimeMinutes
  type: integer
provider_name: Amazon Cloud9
provider_slug: amazon-cloud9
schema_file: json-schema/cloud9-create-environment-ec2-request-schema.json
slug: cloud9-create-environment-ec2-request
source_filename: cloud9-create-environment-ec2-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-create-environment-ec2-request-schema.json\",\n  \"title\": \"CreateEnvironmentEC2Request\",\n  \"description\": \"Request body for creating an EC2-based Cloud9 environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the environment.\",\n      \"example\": \"my-dev-environment\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the environment.\"\n    },\n    \"instanceType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of instance to connect to the environment.\",\n      \"example\": \"t3.small\"\n    },\n    \"connectionType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONNECT_SSH\",\n        \"CONNECT_SSM\"\n \
  \     ],\n      \"description\": \"The connection type to use for connecting to the environment.\"\n    },\n    \"automaticStopTimeMinutes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of minutes until the running instance is shut down after the environment has last been used.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"instanceType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloud9/refs/heads/main/json-schema/cloud9-create-environment-ec2-request-schema.json
tags:
- AWS
- Cloud9
- IDE
- Development
- Browser-Based
title: CreateEnvironmentEC2Request
---
