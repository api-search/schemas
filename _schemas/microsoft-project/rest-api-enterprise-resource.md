---
description: Enterprise resource schema from Microsoft Project Online REST API
layout: schema
name: EnterpriseResource
properties_list:
- description: Resource identifier
  name: Id
  type: string
- description: Resource name
  name: Name
  type: string
- description: Resource email address
  name: Email
  type: string
- description: Resource type (0=Material, 1=Work, 2=Cost)
  name: ResourceType
  type: integer
- description: Whether the resource is active
  name: IsActive
  type: boolean
- description: Whether this is a generic resource
  name: IsGeneric
  type: boolean
- description: Maximum assignment units
  name: MaxUnits
  type: number
- description: Standard billing rate
  name: StandardRate
  type: number
- description: Cost center code
  name: CostCenter
  type: string
- description: Resource group
  name: Group
  type: string
- description: Base calendar name
  name: BaseCalendar
  type: string
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-enterprise-resource-schema.json
slug: rest-api-enterprise-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-enterprise-resource-schema.json\",\n  \"title\": \"EnterpriseResource\",\n  \"description\": \"Enterprise resource schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Resource identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Resource name\"\n    },\n    \"Email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Resource email address\"\n    },\n    \"ResourceType\": {\n      \"type\": \"integer\",\n      \"description\": \"Resource type (0=Material, 1=Work, 2=Cost)\"\n    },\n    \"IsActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the resource\
  \ is active\"\n    },\n    \"IsGeneric\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a generic resource\"\n    },\n    \"MaxUnits\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Maximum assignment units\"\n    },\n    \"StandardRate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Standard billing rate\"\n    },\n    \"CostCenter\": {\n      \"type\": \"string\",\n      \"description\": \"Cost center code\"\n    },\n    \"Group\": {\n      \"type\": \"string\",\n      \"description\": \"Resource group\"\n    },\n    \"BaseCalendar\": {\n      \"type\": \"string\",\n      \"description\": \"Base calendar name\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-enterprise-resource-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: EnterpriseResource
---
