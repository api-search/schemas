---
description: An SSM Parameter Store parameter containing configuration data.
layout: schema
name: Parameter
properties_list:
- description: The name of the parameter.
  name: Name
  type: string
- description: The type of parameter.
  name: Type
  type: string
- description: The parameter value.
  name: Value
  type: string
- description: The parameter version.
  name: Version
  type: integer
- description: The Amazon Resource Name (ARN) of the parameter.
  name: ARN
  type: string
- description: Date the parameter was last changed or updated.
  name: LastModifiedDate
  type: string
- description: The data type of the parameter.
  name: DataType
  type: string
- description: Either the version number or the label used to retrieve the parameter value.
  name: Selector
  type: string
- description: The raw result or response from the source.
  name: SourceResult
  type: string
provider_name: Amazon Systems Manager
provider_slug: amazon-systems-manager
schema_file: json-schema/amazon-systems-manager-parameter-schema.json
slug: amazon-systems-manager-parameter
source_filename: amazon-systems-manager-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An SSM Parameter Store parameter containing configuration data.\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the parameter.\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of parameter.\",\n      \"enum\": [\n        \"String\",\n        \"StringList\",\n        \"SecureString\"\n      ]\n    },\n    \"Value\": {\n      \"type\": \"string\",\n      \"description\": \"The parameter value.\"\n    },\n    \"Version\": {\n      \"type\": \"integer\",\n      \"description\": \"The parameter version.\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the parameter.\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the parameter was last changed or updated.\"\n    },\n    \"DataType\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The data type of the parameter.\"\n    },\n    \"Selector\": {\n      \"type\": \"string\",\n      \"description\": \"Either the version number or the label used to retrieve the parameter value.\"\n    },\n    \"SourceResult\": {\n      \"type\": \"string\",\n      \"description\": \"The raw result or response from the source.\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Type\",\n    \"Value\",\n    \"Version\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Parameter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-systems-manager/refs/heads/main/json-schema/amazon-systems-manager-parameter-schema.json
tags:
- Automation
- AWS
- Management
- Operations
title: Parameter
---
