---
description: A Render cloud service (web service, static site, background worker, cron job, or private service)
layout: schema
name: Render Service
properties_list:
- description: Unique identifier for the service
  name: id
  type: string
- description: Human-readable name of the service
  name: name
  type: string
- description: The type of Render service
  name: type
  type: string
- description: ID of the user or team that owns the service
  name: ownerId
  type: string
- description: ID of the environment the service belongs to
  name: environmentId
  type: string
- description: Git repository URL
  name: repo
  type: string
- description: Git branch to deploy from
  name: branch
  type: string
- description: Root directory for the service build
  name: rootDir
  type: string
- description: Command to build the service
  name: buildCommand
  type: string
- description: Command to start the service
  name: startCommand
  type: string
- description: Service plan tier
  name: plan
  type: string
- description: Deployment region
  name: region
  type: string
- description: Current service status
  name: status
  type: string
- description: URL-friendly slug for the service
  name: slug
  type: string
- description: Service-type-specific configuration details
  name: serviceDetails
  type: object
- description: Autoscaling configuration
  name: autoscaling
  type: object
- description: Timestamp when the service was created
  name: createdAt
  type: string
- description: Timestamp when the service was last updated
  name: updatedAt
  type: string
provider_name: Render
provider_slug: render
schema_file: json-schema/render-service-schema.json
slug: render-service
source_filename: render-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api.render.com/schemas/service\",\n  \"title\": \"Render Service\",\n  \"description\": \"A Render cloud service (web service, static site, background worker, cron job, or private service)\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"type\", \"ownerId\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the service\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the service\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Render service\",\n      \"enum\": [\n        \"web_service\",\n        \"static_site\",\n        \"background_worker\",\n        \"cron_job\",\n        \"private_service\"\n      ]\n    },\n    \"ownerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user or team that\
  \ owns the service\"\n    },\n    \"environmentId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the environment the service belongs to\"\n    },\n    \"repo\": {\n      \"type\": \"string\",\n      \"description\": \"Git repository URL\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Git branch to deploy from\"\n    },\n    \"rootDir\": {\n      \"type\": \"string\",\n      \"description\": \"Root directory for the service build\"\n    },\n    \"buildCommand\": {\n      \"type\": \"string\",\n      \"description\": \"Command to build the service\"\n    },\n    \"startCommand\": {\n      \"type\": \"string\",\n      \"description\": \"Command to start the service\"\n    },\n    \"plan\": {\n      \"type\": \"string\",\n      \"description\": \"Service plan tier\",\n      \"enum\": [\"starter\", \"standard\", \"pro\", \"pro_plus\", \"pro_max\", \"pro_ultra\", \"free\"]\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Deployment region\",\n      \"enum\": [\"oregon\", \"ohio\", \"virginia\", \"frankfurt\", \"singapore\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current service status\",\n      \"enum\": [\"live\", \"not_live\", \"suspended\", \"deactivated\"]\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"URL-friendly slug for the service\"\n    },\n    \"serviceDetails\": {\n      \"type\": \"object\",\n      \"description\": \"Service-type-specific configuration details\",\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"Public URL of the service\"\n        },\n        \"numInstances\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of running instances\"\n        },\n        \"runtime\": {\n          \"type\": \"string\",\n          \"description\": \"Runtime environment (node, python, ruby, go, etc.)\"\n        },\n      \
  \  \"envVars\": {\n          \"type\": \"array\",\n          \"description\": \"Environment variables\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"key\": { \"type\": \"string\" },\n              \"value\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"autoscaling\": {\n      \"type\": \"object\",\n      \"description\": \"Autoscaling configuration\",\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether autoscaling is enabled\"\n        },\n        \"min\": {\n          \"type\": \"integer\",\n          \"description\": \"Minimum number of instances\"\n        },\n        \"max\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of instances\"\n        },\n        \"criteria\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"cpu\": {\n              \"type\"\
  : \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\": \"boolean\" },\n                \"percentage\": { \"type\": \"integer\" }\n              }\n            },\n            \"memory\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"enabled\": { \"type\": \"boolean\" },\n                \"percentage\": { \"type\": \"integer\" }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the service was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the service was last updated\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/render/refs/heads/main/json-schema/render-service-schema.json
tags:
- Cloud
- Platform
- Deployment
- Infrastructure
- DevOps
- Web Services
- Databases
- Hosting
title: Render Service
---
