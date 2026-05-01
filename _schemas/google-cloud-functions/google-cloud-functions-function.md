---
description: Represents a Cloud Function, a lightweight, event-driven serverless compute unit that executes user code in response to events or HTTP requests.
layout: schema
name: Google Cloud Function
properties_list:
- description: Output only. The resource name of the function in the format projects/{project}/locations/{location}/functions/{function}.
  name: name
  type: string
- description: User-provided description of the function.
  name: description
  type: string
- description: The environment the function is hosted on.
  name: environment
  type: string
- description: Describes the build step of the function.
  name: buildConfig
  type: object
- description: Describes the service configuration for the function.
  name: serviceConfig
  type: object
- description: An event trigger configuration.
  name: eventTrigger
  type: object
- description: Output only. State of the function.
  name: state
  type: string
- description: Output only. The last update timestamp of the function.
  name: updateTime
  type: string
- description: Labels associated with this function.
  name: labels
  type: object
- description: Output only. The deployed URL for the function.
  name: url
  type: string
provider_name: Google Cloud Functions
provider_slug: google-cloud-functions
schema_file: json-schema/google-cloud-functions-function-schema.json
slug: google-cloud-functions-function
source_filename: google-cloud-functions-function-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-functions/refs/heads/main/json-schema/google-cloud-functions-function-schema.json\",\n  \"title\": \"Google Cloud Function\",\n  \"description\": \"Represents a Cloud Function, a lightweight, event-driven serverless compute unit that executes user code in response to events or HTTP requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. The resource name of the function in the format projects/{project}/locations/{location}/functions/{function}.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-provided description of the function.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"enum\": [\"ENVIRONMENT_UNSPECIFIED\", \"GEN_1\", \"GEN_2\"],\n      \"description\": \"The environment\
  \ the function is hosted on.\"\n    },\n    \"buildConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the build step of the function.\",\n      \"properties\": {\n        \"runtime\": {\n          \"type\": \"string\",\n          \"description\": \"The runtime in which to run the function.\"\n        },\n        \"entryPoint\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the function entry point.\"\n        },\n        \"source\": {\n          \"type\": \"object\",\n          \"description\": \"Source code location.\",\n          \"properties\": {\n            \"storageSource\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"bucket\": { \"type\": \"string\" },\n                \"object\": { \"type\": \"string\" },\n                \"generation\": { \"type\": \"string\" }\n              }\n            },\n            \"repoSource\": {\n              \"type\": \"object\",\n            \
  \  \"properties\": {\n                \"projectId\": { \"type\": \"string\" },\n                \"repoName\": { \"type\": \"string\" },\n                \"branchName\": { \"type\": \"string\" }\n              }\n            }\n          }\n        },\n        \"dockerRepository\": { \"type\": \"string\" },\n        \"workerPool\": { \"type\": \"string\" },\n        \"environmentVariables\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"serviceConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Describes the service configuration for the function.\",\n      \"properties\": {\n        \"service\": { \"type\": \"string\" },\n        \"timeoutSeconds\": { \"type\": \"integer\" },\n        \"availableMemory\": { \"type\": \"string\" },\n        \"maxInstanceCount\": { \"type\": \"integer\" },\n        \"minInstanceCount\": { \"type\": \"integer\" },\n        \"availableCpu\": { \"type\": \"\
  string\" },\n        \"environmentVariables\": {\n          \"type\": \"object\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        },\n        \"ingressSettings\": {\n          \"type\": \"string\",\n          \"enum\": [\"INGRESS_SETTINGS_UNSPECIFIED\", \"ALLOW_ALL\", \"ALLOW_INTERNAL_ONLY\", \"ALLOW_INTERNAL_AND_GCLB\"]\n        },\n        \"uri\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Output only. URI of the deployed service.\"\n        },\n        \"serviceAccountEmail\": { \"type\": \"string\" }\n      }\n    },\n    \"eventTrigger\": {\n      \"type\": \"object\",\n      \"description\": \"An event trigger configuration.\",\n      \"properties\": {\n        \"eventType\": { \"type\": \"string\" },\n        \"pubsubTopic\": { \"type\": \"string\" },\n        \"serviceAccountEmail\": { \"type\": \"string\" },\n        \"retryPolicy\": {\n          \"type\": \"string\",\n          \"enum\": [\"RETRY_POLICY_UNSPECIFIED\"\
  , \"RETRY_POLICY_DO_NOT_RETRY\", \"RETRY_POLICY_RETRY\"]\n        }\n      }\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"STATE_UNSPECIFIED\", \"ACTIVE\", \"FAILED\", \"DEPLOYING\", \"DELETING\", \"UNKNOWN\"],\n      \"description\": \"Output only. State of the function.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The last update timestamp of the function.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"string\" },\n      \"description\": \"Labels associated with this function.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Output only. The deployed URL for the function.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-functions/refs/heads/main/json-schema/google-cloud-functions-function-schema.json
tags:
- Event-Driven
- Functions
- Google Cloud
- Serverless
title: Google Cloud Function
---
