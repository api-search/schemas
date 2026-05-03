---
description: A normalized schema for a deployment on a scalable PaaS platform such as Vercel, Netlify, Heroku, Fly.io, Railway, or Render.
layout: schema
name: Platform Deployment
properties_list:
- description: Unique deployment identifier assigned by the platform.
  name: id
  type: string
- description: PaaS platform provider.
  name: provider
  type: string
- description: ID of the application/project this deployment belongs to.
  name: appId
  type: string
- description: Human-readable application name.
  name: appName
  type: string
- description: Deployment environment.
  name: environment
  type: string
- description: Current deployment status.
  name: status
  type: string
- description: Public URL for this deployment.
  name: url
  type: string
- description: Source code commit triggering this deployment.
  name: gitCommit
  type: object
- description: Build configuration and outcome.
  name: build
  type: object
- description: Runtime configuration for the deployed application.
  name: runtime
  type: object
- description: Platform-managed scaling configuration.
  name: scaling
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: readyAt
  type: string
provider_name: Scalable Platforms
provider_slug: scalable-platforms
schema_file: json-schema/scalable-platforms-deployment-schema.json
slug: scalable-platforms-deployment
source_filename: scalable-platforms-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-platforms/main/json-schema/scalable-platforms-deployment-schema.json\",\n  \"title\": \"Platform Deployment\",\n  \"description\": \"A normalized schema for a deployment on a scalable PaaS platform such as Vercel, Netlify, Heroku, Fly.io, Railway, or Render.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"provider\", \"appId\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique deployment identifier assigned by the platform.\"\n    },\n    \"provider\": {\n      \"type\": \"string\",\n      \"description\": \"PaaS platform provider.\",\n      \"enum\": [\"vercel\", \"netlify\", \"cloudflare-pages\", \"heroku\", \"fly-io\", \"railway\", \"render\", \"northflank\"]\n    },\n    \"appId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the application/project\
  \ this deployment belongs to.\"\n    },\n    \"appName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable application name.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment environment.\",\n      \"enum\": [\"production\", \"staging\", \"preview\", \"development\"],\n      \"default\": \"preview\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current deployment status.\",\n      \"enum\": [\"queued\", \"building\", \"deploying\", \"ready\", \"failed\", \"cancelled\", \"error\"]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Public URL for this deployment.\"\n    },\n    \"gitCommit\": {\n      \"type\": \"object\",\n      \"description\": \"Source code commit triggering this deployment.\",\n      \"properties\": {\n        \"sha\": {\"type\": \"string\", \"description\": \"Full commit SHA.\"},\n        \"branch\": {\"\
  type\": \"string\"},\n        \"message\": {\"type\": \"string\"},\n        \"author\": {\"type\": \"string\"}\n      }\n    },\n    \"build\": {\n      \"type\": \"object\",\n      \"description\": \"Build configuration and outcome.\",\n      \"properties\": {\n        \"command\": {\"type\": \"string\", \"description\": \"Build command (e.g., npm run build).\"},\n        \"outputDirectory\": {\"type\": \"string\", \"description\": \"Build output directory (e.g., .next, dist, public).\"},\n        \"durationSeconds\": {\"type\": \"number\", \"description\": \"Total build duration.\"},\n        \"logUrl\": {\"type\": \"string\", \"format\": \"uri\", \"description\": \"URL to build logs.\"}\n      }\n    },\n    \"runtime\": {\n      \"type\": \"object\",\n      \"description\": \"Runtime configuration for the deployed application.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"static\", \"serverless\", \"server\", \"edge\", \"\
  container\"],\n          \"description\": \"Execution model.\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"Primary deployment region (e.g., iad1, fra1, us-east-1).\"\n        },\n        \"regions\": {\n          \"type\": \"array\",\n          \"items\": {\"type\": \"string\"},\n          \"description\": \"All regions where the deployment is active.\"\n        },\n        \"memory\": {\n          \"type\": \"integer\",\n          \"description\": \"Memory in MB for function/serverless deployments.\"\n        },\n        \"timeout\": {\n          \"type\": \"integer\",\n          \"description\": \"Execution timeout in seconds.\"\n        }\n      }\n    },\n    \"scaling\": {\n      \"type\": \"object\",\n      \"description\": \"Platform-managed scaling configuration.\",\n      \"properties\": {\n        \"minInstances\": {\"type\": \"integer\", \"minimum\": 0, \"description\": \"Minimum instances; 0 for scale-to-zero.\"},\n    \
  \    \"maxInstances\": {\"type\": \"integer\", \"minimum\": 1},\n        \"scaleToZero\": {\"type\": \"boolean\", \"default\": false}\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"readyAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/json-schema/scalable-platforms-deployment-schema.json
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
title: Platform Deployment
---
