---
description: Schema for a Cloud Build build resource, representing a CI/CD build execution on Google Cloud infrastructure.
layout: schema
name: Google Cloud Build Build
properties_list:
- description: Unique identifier of the build
  name: id
  type: string
- description: ID of the project
  name: projectId
  type: string
- description: Status of the build
  name: status
  type: string
- description: The location of the source files to build
  name: source
  type: object
- description: The operations to be performed on the workspace
  name: steps
  type: array
- description: List of images to be pushed upon successful build completion
  name: images
  type: array
- description: Amount of time that this build should be allowed to run (e.g. 600s)
  name: timeout
  type: string
- description: Substitution variables for the build
  name: substitutions
  type: object
- description: Tags for organizing builds
  name: tags
  type: array
- description: URL to logs for this build in Cloud Console
  name: logUrl
  type: string
- description: Time at which the build was created
  name: createTime
  type: string
- description: Time at which execution of the build was started
  name: startTime
  type: string
- description: Time at which execution of the build was finished
  name: finishTime
  type: string
provider_name: Google Cloud Build
provider_slug: google-cloud-build
schema_file: json-schema/google-cloud-build-build-schema.json
slug: google-cloud-build-build
source_filename: google-cloud-build-build-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/cloudbuild/build.json\",\n  \"title\": \"Google Cloud Build Build\",\n  \"description\": \"Schema for a Cloud Build build resource, representing a CI/CD build execution on Google Cloud infrastructure.\",\n  \"type\": \"object\",\n  \"required\": [\"steps\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the build\"\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the project\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the build\",\n      \"enum\": [\"STATUS_UNKNOWN\", \"PENDING\", \"QUEUED\", \"WORKING\", \"SUCCESS\", \"FAILURE\", \"INTERNAL_ERROR\", \"TIMEOUT\", \"CANCELLED\", \"EXPIRED\"]\n    },\n    \"source\": {\n      \"$ref\": \"#/$defs/Source\",\n      \"description\": \"The location of the source\
  \ files to build\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"The operations to be performed on the workspace\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BuildStep\"\n      },\n      \"minItems\": 1\n    },\n    \"images\": {\n      \"type\": \"array\",\n      \"description\": \"List of images to be pushed upon successful build completion\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"timeout\": {\n      \"type\": \"string\",\n      \"description\": \"Amount of time that this build should be allowed to run (e.g. 600s)\",\n      \"pattern\": \"^[0-9]+s$\"\n    },\n    \"substitutions\": {\n      \"type\": \"object\",\n      \"description\": \"Substitution variables for the build\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags for organizing builds\",\n      \"items\": {\n        \"type\": \"string\"\n\
  \      }\n    },\n    \"logUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to logs for this build in Cloud Console\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which the build was created\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which execution of the build was started\"\n    },\n    \"finishTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which execution of the build was finished\"\n    }\n  },\n  \"$defs\": {\n    \"Source\": {\n      \"type\": \"object\",\n      \"description\": \"Location of the source in a supported storage service\",\n      \"properties\": {\n        \"storageSource\": {\n          \"type\": \"object\",\n          \"description\": \"Source from Cloud Storage\",\n          \"properties\": {\n\
  \            \"bucket\": {\n              \"type\": \"string\",\n              \"description\": \"Cloud Storage bucket containing the source\"\n            },\n            \"object\": {\n              \"type\": \"string\",\n              \"description\": \"Cloud Storage object containing the source\"\n            },\n            \"generation\": {\n              \"type\": \"string\",\n              \"description\": \"Cloud Storage generation for the object\"\n            }\n          }\n        },\n        \"repoSource\": {\n          \"type\": \"object\",\n          \"description\": \"Source from a Cloud Source Repository\",\n          \"properties\": {\n            \"projectId\": {\n              \"type\": \"string\"\n            },\n            \"repoName\": {\n              \"type\": \"string\"\n            },\n            \"branchName\": {\n              \"type\": \"string\"\n            },\n            \"tagName\": {\n              \"type\": \"string\"\n            },\n          \
  \  \"commitSha\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"BuildStep\": {\n      \"type\": \"object\",\n      \"description\": \"A step in the build pipeline\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the container image for this build step\"\n        },\n        \"args\": {\n          \"type\": \"array\",\n          \"description\": \"Command-line arguments to the step's container\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"dir\": {\n          \"type\": \"string\",\n          \"description\": \"Working directory for the step\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the build step\"\n        },\n        \"waitFor\": {\n          \"type\": \"array\",\n          \"description\": \"IDs of steps\
  \ that this step depends on\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"entrypoint\": {\n          \"type\": \"string\",\n          \"description\": \"Entrypoint to use for the step's container\"\n        },\n        \"env\": {\n          \"type\": \"array\",\n          \"description\": \"Environment variables for the step\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Timeout for this build step\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-build/refs/heads/main/json-schema/google-cloud-build-build-schema.json
tags:
- Build Automation
- CI/CD
- Container Build
- Continuous Delivery
- Continuous Integration
- DevOps
title: Google Cloud Build Build
---
