---
description: ConnectorEntity schema from Amazon AppFlow API
layout: schema
name: ConnectorEntity
properties_list:
- description: The name of the connector entity.
  name: name
  type: string
- description: The label applied to the connector entity.
  name: label
  type: string
- description: Specifies whether the connector entity is a parent or a category and has more entities nested underneath it.
  name: hasNestedEntities
  type: boolean
provider_name: Amazon AppFlow
provider_slug: amazon-appflow
schema_file: json-schema/appflow-connector-entity-schema.json
slug: appflow-connector-entity
source_filename: appflow-connector-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-entity-schema.json\",\n  \"title\": \"ConnectorEntity\",\n  \"description\": \"ConnectorEntity schema from Amazon AppFlow API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Account\",\n      \"description\": \"The name of the connector entity.\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Account\",\n      \"description\": \"The label applied to the connector entity.\"\n    },\n    \"hasNestedEntities\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Specifies whether the connector entity is a parent or a category and has more entities nested underneath it.\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-appflow/refs/heads/main/json-schema/appflow-connector-entity-schema.json
tags:
- AWS
- Connectors
- Data Flow
- Data Integration
- ETL
- Integration
- SaaS
- Data Transfer
title: ConnectorEntity
---
