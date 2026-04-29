---
description: Schema representing a Convex deployment, which is a runtime environment where Convex backend functions execute. Deployments have a unique name that forms the subdomain of their URL (e.g. happy-otter-123.convex.cloud). Each deployment has its own database, file storage, scheduled functions, and environment variable configuration.
layout: schema
name: Convex Deployment
properties_list:
- description: Unique integer identifier for the deployment assigned by Convex.
  name: id
  type: integer
- description: Unique name of the deployment used as the subdomain of the deployment URL (e.g. 'happy-otter-123').
  name: name
  type: string
- description: The type of deployment environment, determining its lifecycle and usage context.
  name: deployment_type
  type: string
- description: The compute class determining resource limits (memory, concurrency) and pricing tier.
  name: deployment_class
  type: string
- description: The cloud region where this deployment runs.
  name: region
  type: string
- description: ID of the project that owns this deployment.
  name: project_id
  type: integer
- description: The base HTTPS URL of the deployment in the format https://{name}.convex.cloud.
  name: url
  type: string
- description: Environment variables configured for this deployment, accessible to backend functions at runtime via process.env.
  name: environment_variables
  type: array
- description: Custom domain names associated with this deployment.
  name: custom_domains
  type: array
provider_name: Convex
provider_slug: convex
schema_file: json-schema/convex-deployment-schema.json
slug: convex-deployment
source_filename: convex-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://convex.dev/schemas/convex/deployment.json\",\n  \"title\": \"Convex Deployment\",\n  \"description\": \"Schema representing a Convex deployment, which is a runtime environment where Convex backend functions execute. Deployments have a unique name that forms the subdomain of their URL (e.g. happy-otter-123.convex.cloud). Each deployment has its own database, file storage, scheduled functions, and environment variable configuration.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"deployment_type\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique integer identifier for the deployment assigned by Convex.\",\n      \"minimum\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the deployment used as the subdomain of the deployment URL (e.g. 'happy-otter-123').\",\n      \"pattern\"\
  : \"^[a-z0-9-]+$\"\n    },\n    \"deployment_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of deployment environment, determining its lifecycle and usage context.\",\n      \"enum\": [\"dev\", \"prod\", \"preview\", \"custom\"]\n    },\n    \"deployment_class\": {\n      \"type\": \"string\",\n      \"description\": \"The compute class determining resource limits (memory, concurrency) and pricing tier.\",\n      \"enum\": [\"s16\", \"s256\", \"d1024\"]\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud region where this deployment runs.\",\n      \"enum\": [\"aws-us-east-1\", \"aws-eu-west-1\"]\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the project that owns this deployment.\",\n      \"minimum\": 1\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The base HTTPS URL of the deployment in the format https://{name}.convex.cloud.\"\
  ,\n      \"pattern\": \"^https://[a-z0-9-]+\\\\.convex\\\\.cloud$\"\n    },\n    \"environment_variables\": {\n      \"type\": \"array\",\n      \"description\": \"Environment variables configured for this deployment, accessible to backend functions at runtime via process.env.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/EnvironmentVariable\"\n      }\n    },\n    \"custom_domains\": {\n      \"type\": \"array\",\n      \"description\": \"Custom domain names associated with this deployment.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CustomDomain\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"EnvironmentVariable\": {\n      \"type\": \"object\",\n      \"description\": \"A key-value environment variable configured on a Convex deployment. Environment variables are accessible to all backend functions at runtime.\",\n      \"required\": [\"name\", \"value\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The environment\
  \ variable key name following standard naming conventions.\",\n          \"pattern\": \"^[A-Za-z_][A-Za-z0-9_]*$\",\n          \"examples\": [\"DATABASE_URL\", \"API_KEY\", \"WEBHOOK_SECRET\"]\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The environment variable value. May contain connection strings, API keys, or other configuration data.\",\n          \"maxLength\": 8192\n        }\n      }\n    },\n    \"CustomDomain\": {\n      \"type\": \"object\",\n      \"description\": \"A custom domain name associated with a Convex deployment for routing external traffic.\",\n      \"required\": [\"domain\", \"request_destination\"],\n      \"properties\": {\n        \"domain\": {\n          \"type\": \"string\",\n          \"description\": \"The fully-qualified custom domain name (e.g. 'api.example.com').\",\n          \"format\": \"hostname\"\n        },\n        \"request_destination\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Routing destination for requests to this domain. convexCloud routes to the function API (queries, mutations, actions); convexSite routes to HTTP action endpoints.\",\n          \"enum\": [\"convexCloud\", \"convexSite\"]\n        }\n      }\n    },\n    \"DeployKey\": {\n      \"type\": \"object\",\n      \"description\": \"A deploy key used to authenticate the Convex CLI or CI/CD pipelines when pushing function code to a deployment.\",\n      \"required\": [\"name\", \"deployment_name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable name for the deploy key.\"\n        },\n        \"deployment_name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the deployment this key is scoped to.\",\n          \"pattern\": \"^[a-z0-9-]+$\"\n        },\n        \"key\": {\n          \"type\": \"string\",\n          \"description\": \"The deploy key value. Only present immediately after creation;\
  \ not returned by subsequent list operations.\",\n          \"pattern\": \"^prod:[A-Za-z0-9_-]+$\"\n        },\n        \"created_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this deploy key was created.\"\n        }\n      }\n    },\n    \"Project\": {\n      \"type\": \"object\",\n      \"description\": \"A Convex project, which is the top-level organizational unit grouping related deployments.\",\n      \"required\": [\"id\", \"slug\", \"name\", \"team_id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique integer identifier for the project.\",\n          \"minimum\": 1\n        },\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable URL-safe identifier for the project within the team.\",\n          \"pattern\": \"^[a-z0-9-]+$\"\n        },\n        \"name\": {\n          \"type\": \"\
  string\",\n          \"description\": \"Display name of the project.\",\n          \"maxLength\": 128\n        },\n        \"team_id\": {\n          \"type\": \"integer\",\n          \"description\": \"ID of the team that owns this project.\",\n          \"minimum\": 1\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/convex/refs/heads/main/json-schema/convex-deployment-schema.json
tags:
- Backend
- Database
- Functions
- Real-Time
- Reactive
- Serverless
- TypeScript
title: Convex Deployment
---
