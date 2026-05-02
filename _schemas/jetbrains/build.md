---
description: A build resource in JetBrains TeamCity CI/CD server.
layout: schema
name: JetBrains TeamCity Build
properties_list:
- description: Unique numeric identifier of the build.
  name: id
  type: integer
- description: Build number string.
  name: number
  type: string
- description: Status of the build.
  name: status
  type: string
- description: Current state of the build.
  name: state
  type: string
- description: Branch name the build ran on.
  name: branchName
  type: string
- description: Identifier of the build configuration.
  name: buildTypeId
  type: string
- description: Timestamp when the build started.
  name: startDate
  type: string
- description: Timestamp when the build finished.
  name: finishDate
  type: string
- description: Timestamp when the build was queued.
  name: queuedDate
  type: string
- description: Information about what triggered the build.
  name: triggered
  type: object
- description: Build agent that ran the build.
  name: agent
  type: object
- description: Summary of test results.
  name: testOccurrences
  type: object
provider_name: JetBrains
provider_slug: jetbrains
schema_file: json-schema/build.json
slug: build
source_filename: build.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jetbrains-build.json\",\n  \"title\": \"JetBrains TeamCity Build\",\n  \"description\": \"A build resource in JetBrains TeamCity CI/CD server.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier of the build.\"\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"Build number string.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"SUCCESS\", \"FAILURE\", \"ERROR\", \"UNKNOWN\"],\n      \"description\": \"Status of the build.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"queued\", \"running\", \"finished\"],\n      \"description\": \"Current state of the build.\"\n    },\n    \"branchName\": {\n      \"type\": \"string\",\n      \"description\": \"Branch name the build ran on.\"\n    },\n    \"buildTypeId\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Identifier of the build configuration.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the build started.\"\n    },\n    \"finishDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the build finished.\"\n    },\n    \"queuedDate\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the build was queued.\"\n    },\n    \"triggered\": {\n      \"type\": \"object\",\n      \"description\": \"Information about what triggered the build.\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\" },\n        \"date\": { \"type\": \"string\" }\n      }\n    },\n    \"agent\": {\n      \"type\": \"object\",\n      \"description\": \"Build agent that ran the build.\",\n      \"properties\": {\n        \"id\": { \"type\": \"integer\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"testOccurrences\": {\n     \
  \ \"type\": \"object\",\n      \"description\": \"Summary of test results.\",\n      \"properties\": {\n        \"count\": { \"type\": \"integer\" },\n        \"passed\": { \"type\": \"integer\" },\n        \"failed\": { \"type\": \"integer\" }\n      }\n    }\n  },\n  \"required\": [\"id\", \"status\", \"state\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/json-schema/build.json
tags:
- CI/CD
- Developer Tools
- IDE
title: JetBrains TeamCity Build
---
