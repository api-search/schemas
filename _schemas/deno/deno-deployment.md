---
description: Represents a Deno Deploy deployment, which is an immutable unit of code, static assets, environment variables, and configuration that runs on Deno Deploy edge infrastructure. Deployments are created from a set of assets and an entry point, and become active when attached to a domain or project subdomain. In the v2 API, deployments are called revisions.
layout: schema
name: Deno Deployment
properties_list:
- description: Unique identifier for the deployment, assigned by Deno Deploy at creation time
  name: id
  type: string
- description: UUID of the project that owns this deployment
  name: projectId
  type: string
- description: Current lifecycle status of the deployment
  name: status
  type: string
- description: List of custom domain names currently serving traffic from this deployment
  name: domains
  type: array
- description: Environment variables configured for this deployment. Secret variable values are redacted in API responses.
  name: envVars
  type: object
- description: Deno KV database associations for this deployment, keyed by the binding name used within the deployment code
  name: databases
  type: object
- description: Map of file paths to asset definitions included in this deployment
  name: assets
  type: object
- description: Relative path to the main entry point module within the assets, executed when the deployment receives a request
  name: entryPointUrl
  type: string
- description: ''
  name: compilerOptions
  type: object
- description: ISO 8601 UTC timestamp when the deployment was created
  name: createdAt
  type: string
- description: ISO 8601 UTC timestamp when the deployment was last modified
  name: updatedAt
  type: string
provider_name: Deno
provider_slug: deno
schema_file: json-schema/deno-deployment-schema.json
slug: deno-deployment
source_filename: deno-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/deno/schemas/deno/deployment.json\",\n  \"title\": \"Deno Deployment\",\n  \"description\": \"Represents a Deno Deploy deployment, which is an immutable unit of code, static assets, environment variables, and configuration that runs on Deno Deploy edge infrastructure. Deployments are created from a set of assets and an entry point, and become active when attached to a domain or project subdomain. In the v2 API, deployments are called revisions.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"projectId\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the deployment, assigned by Deno Deploy at creation time\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"UUID of the project that owns this deployment\"\n    },\n\
  \    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle status of the deployment\",\n      \"enum\": [\"pending\", \"failed\", \"success\"]\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"List of custom domain names currently serving traffic from this deployment\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"A fully qualified domain name attached to this deployment\"\n      }\n    },\n    \"envVars\": {\n      \"type\": \"object\",\n      \"description\": \"Environment variables configured for this deployment. Secret variable values are redacted in API responses.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"databases\": {\n      \"type\": \"object\",\n      \"description\": \"Deno KV database associations for this deployment, keyed by the binding name used within the deployment code\",\n      \"additionalProperties\": {\n        \"type\"\
  : \"string\",\n        \"format\": \"uuid\",\n        \"description\": \"UUID of an associated Deno KV database\"\n      }\n    },\n    \"assets\": {\n      \"type\": \"object\",\n      \"description\": \"Map of file paths to asset definitions included in this deployment\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/DeploymentAsset\"\n      }\n    },\n    \"entryPointUrl\": {\n      \"type\": \"string\",\n      \"description\": \"Relative path to the main entry point module within the assets, executed when the deployment receives a request\"\n    },\n    \"compilerOptions\": {\n      \"$ref\": \"#/$defs/CompilerOptions\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the deployment was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the deployment was last modified\"\
  \n    }\n  },\n  \"$defs\": {\n    \"DeploymentAsset\": {\n      \"type\": \"object\",\n      \"description\": \"An individual file asset included in a Deno Deploy deployment. Assets can be UTF-8 text files, base64-encoded binary files, references to previously uploaded git blob objects by SHA-1 hash, or symbolic links.\",\n      \"required\": [\"kind\"],\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"The asset type, determining how the content field is interpreted\",\n          \"enum\": [\"file\", \"symlink\"]\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The file content as a UTF-8 string (for text files) or a base64-encoded string (for binary files). Not used for symlink assets.\"\n        },\n        \"encoding\": {\n          \"type\": \"string\",\n          \"description\": \"The encoding of the content field for file assets\",\n          \"enum\": [\"utf-8\", \"base64\"\
  ]\n        },\n        \"gitSha1\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-1 hash of a previously uploaded git blob object. When provided, the content and encoding fields are ignored and the blob content is used instead.\",\n          \"pattern\": \"^[0-9a-f]{40}$\",\n          \"minLength\": 40,\n          \"maxLength\": 40\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"Target path for symlink assets, relative to the project root\"\n        }\n      }\n    },\n    \"CompilerOptions\": {\n      \"type\": \"object\",\n      \"description\": \"TypeScript compiler options applied when building a Deno Deploy deployment\",\n      \"properties\": {\n        \"jsx\": {\n          \"type\": \"string\",\n          \"description\": \"JSX transform mode controlling how JSX syntax is compiled\",\n          \"enum\": [\"react\", \"react-jsx\", \"react-jsxdev\", \"preserve\"]\n        },\n        \"jsxFactory\": {\n   \
  \       \"type\": \"string\",\n          \"description\": \"The function called to create JSX elements (default: React.createElement)\"\n        },\n        \"jsxFragmentFactory\": {\n          \"type\": \"string\",\n          \"description\": \"The function called to create JSX fragments (default: React.Fragment)\"\n        },\n        \"jsxImportSource\": {\n          \"type\": \"string\",\n          \"description\": \"Module specifier used as the source for the JSX automatic runtime\"\n        }\n      }\n    },\n    \"BuildLogEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A single entry from a deployment's build log, capturing output from the compilation and bundling process\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"description\": \"Log severity level\",\n          \"enum\": [\"debug\", \"info\", \"warning\", \"error\"]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Log message content produced during the build\"\n        },\n        \"ts\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this build log entry was produced\"\n        }\n      }\n    },\n    \"AppLogEntry\": {\n      \"type\": \"object\",\n      \"description\": \"A single runtime application log entry emitted by a running deployment. Entries are produced by console.log and related calls within the deployed code.\",\n      \"properties\": {\n        \"level\": {\n          \"type\": \"string\",\n          \"description\": \"Log severity level\",\n          \"enum\": [\"debug\", \"info\", \"warning\", \"error\"]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Log message content\"\n        },\n        \"region\": {\n          \"type\": \"string\",\n          \"description\": \"Deno Deploy region identifier where this log entry was produced (e.g., us-east-1)\"\
  \n        },\n        \"deploymentId\": {\n          \"type\": \"string\",\n          \"description\": \"Identifier of the deployment that produced this log entry\"\n        },\n        \"ts\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when this log entry was produced\"\n        }\n      }\n    },\n    \"DeploymentEvent\": {\n      \"type\": \"object\",\n      \"description\": \"A system-level event recorded in deployment logs. Events capture significant runtime lifecycle occurrences such as isolate boot, memory limit exceeded, or CPU time limit exceeded.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type of deployment event\",\n          \"enum\": [\"boot\", \"memory_limit\", \"cpu_time_limit\"]\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable\
  \ event message, for example 'isolate start time: 96.67 ms (user time: 6.13 ms)'\"\n        },\n        \"urn\": {\n          \"type\": \"string\",\n          \"description\": \"Optional URN for cross-referencing with observability artifacts, present on limit events\"\n        },\n        \"ts\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"ISO 8601 timestamp when the event occurred\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/deno/refs/heads/main/json-schema/deno-deployment-schema.json
tags:
- Deployment
- Edge
- JavaScript
- Runtime
- Serverless
- TypeScript
title: Deno Deployment
---
