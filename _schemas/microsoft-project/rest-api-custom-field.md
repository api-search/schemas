---
description: Custom field schema from Microsoft Project Online REST API
layout: schema
name: CustomField
properties_list:
- description: Custom field identifier
  name: Id
  type: string
- description: Internal name of the custom field
  name: InternalName
  type: string
- description: Display name of the custom field
  name: Name
  type: string
- description: Field data type (0=Cost, 1=Date, 2=Duration, 3=Finish, 4=Flag, 5=Number, 6=Start, 7=Text)
  name: FieldType
  type: integer
- description: Entity type (0=Project, 1=Resource, 2=Task)
  name: EntityType
  type: integer
- description: Field description
  name: Description
  type: string
- description: Associated lookup table ID
  name: LookupTableId
  type: string
- description: Whether the field is required
  name: IsRequired
  type: boolean
- description: Whether the text field supports multiple lines
  name: IsMultilineText
  type: boolean
- description: Calculated field formula
  name: Formula
  type: string
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-custom-field-schema.json
slug: rest-api-custom-field
source_filename: rest-api-custom-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-custom-field-schema.json\",\n  \"title\": \"CustomField\",\n  \"description\": \"Custom field schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Custom field identifier\"\n    },\n    \"InternalName\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the custom field\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the custom field\"\n    },\n    \"FieldType\": {\n      \"type\": \"integer\",\n      \"description\": \"Field data type (0=Cost, 1=Date, 2=Duration, 3=Finish, 4=Flag, 5=Number, 6=Start, 7=Text)\"\n    },\n    \"EntityType\": {\n      \"type\": \"integer\",\n      \"\
  description\": \"Entity type (0=Project, 1=Resource, 2=Task)\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Field description\"\n    },\n    \"LookupTableId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated lookup table ID\"\n    },\n    \"IsRequired\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the field is required\"\n    },\n    \"IsMultilineText\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the text field supports multiple lines\"\n    },\n    \"Formula\": {\n      \"type\": \"string\",\n      \"description\": \"Calculated field formula\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-custom-field-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: CustomField
---
