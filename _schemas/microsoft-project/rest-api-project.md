---
description: Project schema from Microsoft Project Online REST API
layout: schema
name: Project
properties_list:
- description: Unique identifier of the project
  name: Id
  type: string
- description: Name of the project
  name: Name
  type: string
- description: Description of the project
  name: Description
  type: string
- description: Project start date
  name: StartDate
  type: string
- description: Project finish date
  name: FinishDate
  type: string
- description: Date the project was created
  name: CreatedDate
  type: string
- description: Date the project was last modified
  name: ModifiedDate
  type: string
- description: Whether the project is currently checked out
  name: IsCheckedOut
  type: boolean
- description: User who checked out the project
  name: CheckedOutBy
  type: string
- description: Overall completion percentage
  name: PercentComplete
  type: integer
- description: Enterprise project type identifier
  name: ProjectType
  type: integer
- description: URL to the project site
  name: ProjectSiteUrl
  type: string
provider_name: Microsoft Project
provider_slug: microsoft-project
schema_file: json-schema/rest-api-project-schema.json
slug: rest-api-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-project-schema.json\",\n  \"title\": \"Project\",\n  \"description\": \"Project schema from Microsoft Project Online REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of the project\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the project\"\n    },\n    \"StartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Project start date\"\n    },\n    \"FinishDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Project finish\
  \ date\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the project was created\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the project was last modified\"\n    },\n    \"IsCheckedOut\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is currently checked out\"\n    },\n    \"CheckedOutBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who checked out the project\"\n    },\n    \"PercentComplete\": {\n      \"type\": \"integer\",\n      \"description\": \"Overall completion percentage\"\n    },\n    \"ProjectType\": {\n      \"type\": \"integer\",\n      \"description\": \"Enterprise project type identifier\"\n    },\n    \"ProjectSiteUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the project site\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-project/refs/heads/main/json-schema/rest-api-project-schema.json
tags:
- Budgeting
- Gantt Charts
- Microsoft
- Portfolio Management
- Project Management
- Resource Management
- Scheduling
- Task Management
title: Project
---
