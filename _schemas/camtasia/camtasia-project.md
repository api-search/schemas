---
description: Represents a Camtasia video editing project, including canvas settings, timeline configuration, and production metadata.
layout: schema
name: Camtasia Project
properties_list:
- description: Unique identifier for the project
  name: id
  type: string
- description: Project name
  name: name
  type: string
- description: Project description
  name: description
  type: string
- description: Current project status
  name: status
  type: string
- description: Project canvas resolution
  name: resolution
  type: object
- description: Project frame rate in frames per second
  name: frameRate
  type: number
- description: Total project duration in seconds
  name: duration
  type: number
- description: Number of timeline tracks
  name: trackCount
  type: integer
- description: ID of the template used to create this project
  name: templateId
  type: string
- description: When the project was created
  name: createdAt
  type: string
- description: When the project was last modified
  name: updatedAt
  type: string
provider_name: Camtasia
provider_slug: camtasia
schema_file: json-schema/camtasia-project-schema.json
slug: camtasia-project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.techsmith.com/schemas/camtasia/project.json\",\n  \"title\": \"Camtasia Project\",\n  \"description\": \"Represents a Camtasia video editing project, including canvas settings, timeline configuration, and production metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the project\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Project name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Project description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"draft\",\n        \"in_progress\",\n        \"completed\",\n        \"archived\"\n      ],\n      \"description\": \"Current project status\"\n    },\n    \"resolution\": {\n      \"type\": \"object\",\n      \"properties\"\
  : {\n        \"width\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Canvas width in pixels\"\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Canvas height in pixels\"\n        }\n      },\n      \"description\": \"Project canvas resolution\"\n    },\n    \"frameRate\": {\n      \"type\": \"number\",\n      \"minimum\": 1,\n      \"description\": \"Project frame rate in frames per second\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Total project duration in seconds\"\n    },\n    \"trackCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of timeline tracks\"\n    },\n    \"templateId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the template used to create this project\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n    \
  \  \"format\": \"date-time\",\n      \"description\": \"When the project was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the project was last modified\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/json-schema/camtasia-project-schema.json
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
title: Camtasia Project
---
