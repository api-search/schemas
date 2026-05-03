---
description: A deployment of a Render service, representing a specific build and release cycle
layout: schema
name: Render Deploy
properties_list:
- description: Unique identifier for the deploy
  name: id
  type: string
- description: Git commit information for the deploy
  name: commit
  type: object
- description: Current deploy status
  name: status
  type: string
- description: What triggered the deploy
  name: trigger
  type: string
- description: Timestamp when the deploy was initiated
  name: createdAt
  type: string
- description: Timestamp when the deploy status last changed
  name: updatedAt
  type: string
- description: Timestamp when the deploy completed
  name: finishedAt
  type: string
provider_name: Render
provider_slug: render
schema_file: json-schema/render-deploy-schema.json
slug: render-deploy
source_filename: render-deploy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api.render.com/schemas/deploy\",\n  \"title\": \"Render Deploy\",\n  \"description\": \"A deployment of a Render service, representing a specific build and release cycle\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the deploy\"\n    },\n    \"commit\": {\n      \"type\": \"object\",\n      \"description\": \"Git commit information for the deploy\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Git commit SHA\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Git commit message\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Commit timestamp\"\n        }\n  \
  \    }\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current deploy status\",\n      \"enum\": [\n        \"created\",\n        \"build_in_progress\",\n        \"update_in_progress\",\n        \"live\",\n        \"deactivated\",\n        \"build_failed\",\n        \"update_failed\",\n        \"canceled\",\n        \"pre_deploy_in_progress\",\n        \"pre_deploy_failed\"\n      ]\n    },\n    \"trigger\": {\n      \"type\": \"string\",\n      \"description\": \"What triggered the deploy\",\n      \"enum\": [\"api\", \"manual\", \"github\", \"gitlab\", \"bitbucket\", \"auto_rollback\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deploy was initiated\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deploy status last changed\"\n    },\n    \"finishedAt\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deploy completed\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/render/refs/heads/main/json-schema/render-deploy-schema.json
tags:
- Cloud
- Platform
- Deployment
- Infrastructure
- DevOps
- Web Services
- Databases
- Hosting
title: Render Deploy
---
