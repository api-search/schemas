---
description: Task schema from Amazon AppFlow API
layout: schema
name: Task
properties_list:
- description: The source fields to which a particular task is applied.
  name: sourceFields
  type: array
- description: The operation to be performed on the provided source fields.
  name: connectorOperator
  type: object
- description: A field in a destination connector, or a field value against which Amazon AppFlow validates a source field.
  name: destinationField
  type: string
- description: Specifies the particular task implementation that Amazon AppFlow performs.
  name: taskType
  type: string
- description: A map used to store task-related information.
  name: taskProperties
  type: object
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-task-schema.json
slug: appflow-task
source_filename: appflow-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-task-schema.json\",\n  \"title\": \"Task\",\n  \"description\": \"Task schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceFields\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"example\": \"\"\n      },\n      \"example\": [\n        \"Id\",\n        \"Name\"\n      ],\n      \"description\": \"The source fields to which a particular task is applied.\"\n    },\n    \"connectorOperator\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"Salesforce\": \"NO_OP\"\n      },\n      \"description\": \"The operation to be performed on the provided source fields.\"\n    },\n    \"destinationField\": {\n      \"type\": \"string\",\n      \"example\": \"AccountId\",\n      \"description\": \"A field in a\
  \ destination connector, or a field value against which Amazon AppFlow validates a source field.\"\n    },\n    \"taskType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Arithmetic\",\n        \"Filter\",\n        \"Map\",\n        \"Map_all\",\n        \"Mask\",\n        \"Merge\",\n        \"Partition\",\n        \"Passthrough\",\n        \"Truncate\",\n        \"Validate\",\n        \"Concat\"\n      ],\n      \"example\": \"Map\",\n      \"description\": \"Specifies the particular task implementation that Amazon AppFlow performs.\"\n    },\n    \"taskProperties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"SOURCE_DATA_TYPE\": \"string\"\n      },\n      \"description\": \"A map used to store task-related information.\"\n    }\n  },\n  \"required\": [\n    \"taskType\",\n    \"sourceFields\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-task-schema.json
tags:
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: Task
---
