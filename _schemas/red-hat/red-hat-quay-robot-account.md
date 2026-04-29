---
description: A robot account for automated registry access.
layout: schema
name: RobotAccount
properties_list:
- description: The fully qualified name of the robot account.
  name: name
  type: string
- description: A description of the robot account.
  name: description
  type: string
- description: The authentication token for the robot account.
  name: token
  type: string
- description: When the robot account was created.
  name: created
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-quay-robot-account-schema.json
slug: red-hat-quay-robot-account
source_filename: red-hat-quay-robot-account-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RobotAccount\",\n  \"type\": \"object\",\n  \"description\": \"A robot account for automated registry access.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified name of the robot account.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the robot account.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The authentication token for the robot account.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"description\": \"When the robot account was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-quay-robot-account-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: RobotAccount
---
