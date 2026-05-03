---
description: Describes a serverless function (edge function, cloud function, or worker) deployed on scalable platforms such as Vercel Edge Functions, Netlify Functions, Cloudflare Workers, Heroku Functions, Fly.io Machines, or Railway services.
layout: schema
name: Serverless Function
properties_list:
- description: Platform-assigned unique identifier for the function.
  name: id
  type: string
- description: Function name used in deployment and routing.
  name: name
  type: string
- description: Platform hosting the serverless function.
  name: platform
  type: string
- description: Runtime environment for the function.
  name: runtime
  type: string
- description: Entry point file and exported function (e.g., api/hello.js for Next.js API routes).
  name: handler
  type: string
- description: URL path pattern this function handles.
  name: route
  type: string
- description: Deployment region or 'edge' for globally distributed execution.
  name: region
  type: string
- description: Memory allocated to the function in megabytes.
  name: memoryMB
  type: integer
- description: Maximum execution duration before the function is terminated.
  name: timeoutSeconds
  type: integer
- description: Maximum concurrent executions (platform-specific).
  name: maxConcurrency
  type: integer
- description: Whether the function scales to zero when not in use.
  name: scaleToZero
  type: boolean
- description: Environment variables available to the function at runtime.
  name: environment
  type: object
- description: Events that invoke this function.
  name: triggers
  type: array
- description: Deployment timestamp.
  name: deployedAt
  type: string
- description: Current function status.
  name: status
  type: string
provider_name: Scalable Platforms
provider_slug: scalable-platforms
schema_file: json-schema/scalable-platforms-serverless-function-schema.json
slug: scalable-platforms-serverless-function
source_filename: scalable-platforms-serverless-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/scalable-platforms/main/json-schema/scalable-platforms-serverless-function-schema.json\",\n  \"title\": \"Serverless Function\",\n  \"description\": \"Describes a serverless function (edge function, cloud function, or worker) deployed on scalable platforms such as Vercel Edge Functions, Netlify Functions, Cloudflare Workers, Heroku Functions, Fly.io Machines, or Railway services.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"runtime\", \"handler\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Platform-assigned unique identifier for the function.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Function name used in deployment and routing.\",\n      \"pattern\": \"^[a-z][a-z0-9-_]*$\",\n      \"minLength\": 1,\n      \"maxLength\": 64\n    },\n    \"platform\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Platform hosting the serverless function.\",\n      \"enum\": [\"vercel\", \"netlify\", \"cloudflare-workers\", \"heroku\", \"fly-io\", \"railway\", \"render\", \"northflank\"]\n    },\n    \"runtime\": {\n      \"type\": \"string\",\n      \"description\": \"Runtime environment for the function.\",\n      \"enum\": [\n        \"nodejs18\",\n        \"nodejs20\",\n        \"nodejs22\",\n        \"python3.11\",\n        \"python3.12\",\n        \"go1.21\",\n        \"ruby3.3\",\n        \"deno\",\n        \"bun\",\n        \"edge-runtime\",\n        \"workerd\"\n      ]\n    },\n    \"handler\": {\n      \"type\": \"string\",\n      \"description\": \"Entry point file and exported function (e.g., api/hello.js for Next.js API routes).\",\n      \"example\": \"api/hello.js\"\n    },\n    \"route\": {\n      \"type\": \"string\",\n      \"description\": \"URL path pattern this function handles.\",\n      \"example\": \"/api/hello\"\
  \n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment region or 'edge' for globally distributed execution.\",\n      \"examples\": [\"us-east-1\", \"eu-west-1\", \"edge\", \"global\"],\n      \"default\": \"edge\"\n    },\n    \"memoryMB\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory allocated to the function in megabytes.\",\n      \"minimum\": 128,\n      \"maximum\": 3008,\n      \"default\": 256\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum execution duration before the function is terminated.\",\n      \"minimum\": 1,\n      \"maximum\": 900,\n      \"default\": 30\n    },\n    \"maxConcurrency\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum concurrent executions (platform-specific).\",\n      \"minimum\": 1\n    },\n    \"scaleToZero\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the function scales to zero when not in use.\"\
  ,\n      \"default\": true\n    },\n    \"environment\": {\n      \"type\": \"object\",\n      \"description\": \"Environment variables available to the function at runtime.\",\n      \"additionalProperties\": {\"type\": \"string\"}\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"Events that invoke this function.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"type\"],\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"http\", \"cron\", \"queue\", \"event\", \"webhook\"]\n          },\n          \"schedule\": {\n            \"type\": \"string\",\n            \"description\": \"Cron schedule expression (for cron triggers).\",\n            \"example\": \"0 */6 * * *\"\n          },\n          \"method\": {\n            \"type\": \"string\",\n            \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\", \"ANY\"],\n            \"description\": \"HTTP method\
  \ (for http triggers).\"\n          }\n        }\n      }\n    },\n    \"deployedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Deployment timestamp.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current function status.\",\n      \"enum\": [\"active\", \"deploying\", \"failed\", \"paused\"],\n      \"default\": \"active\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/scalable-platforms/refs/heads/main/json-schema/scalable-platforms-serverless-function-schema.json
tags:
- Cloud Infrastructure
- Deployment
- Developer Experience
- DevOps
- PaaS
- Platform
- Scalability
- Serverless
title: Serverless Function
---
