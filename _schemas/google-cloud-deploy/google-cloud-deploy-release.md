---
description: Schema for a Cloud Deploy release, representing a specific version of an application to be deployed through a delivery pipeline.
layout: schema
name: Google Cloud Deploy Release
properties_list:
- description: The resource name of the release
  name: name
  type: string
- description: Description of the release
  name: description
  type: string
- description: User annotations for the release
  name: annotations
  type: object
- description: Labels applied to the release
  name: labels
  type: object
- description: Cloud Storage URI of the Skaffold configuration
  name: skaffoldConfigUri
  type: string
- description: Filepath of the Skaffold config inside the config URI
  name: skaffoldConfigPath
  type: string
- description: List of build artifacts to deploy
  name: buildArtifacts
  type: array
- description: Snapshot of the delivery pipeline at the time of release creation
  name: deliveryPipelineSnapshot
  type: object
- description: Snapshots of targets at the time of release creation
  name: targetSnapshots
  type: array
- description: The current state of the render operation
  name: renderState
  type: string
- description: Time at which the release was created
  name: createTime
  type: string
- description: Time at which the render began
  name: renderStartTime
  type: string
- description: Time at which the render completed
  name: renderEndTime
  type: string
provider_name: Google Cloud Deploy
provider_slug: google-cloud-deploy
schema_file: json-schema/google-cloud-deploy-release-schema.json
slug: google-cloud-deploy-release
source_filename: google-cloud-deploy-release-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/clouddeploy/release.json\",\n  \"title\": \"Google Cloud Deploy Release\",\n  \"description\": \"Schema for a Cloud Deploy release, representing a specific version of an application to be deployed through a delivery pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the release\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the release\"\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"User annotations for the release\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Labels applied to the release\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\
  \n      }\n    },\n    \"skaffoldConfigUri\": {\n      \"type\": \"string\",\n      \"description\": \"Cloud Storage URI of the Skaffold configuration\"\n    },\n    \"skaffoldConfigPath\": {\n      \"type\": \"string\",\n      \"description\": \"Filepath of the Skaffold config inside the config URI\"\n    },\n    \"buildArtifacts\": {\n      \"type\": \"array\",\n      \"description\": \"List of build artifacts to deploy\",\n      \"items\": {\n        \"$ref\": \"#/$defs/BuildArtifact\"\n      }\n    },\n    \"deliveryPipelineSnapshot\": {\n      \"$ref\": \"#/$defs/DeliveryPipelineSnapshot\",\n      \"description\": \"Snapshot of the delivery pipeline at the time of release creation\"\n    },\n    \"targetSnapshots\": {\n      \"type\": \"array\",\n      \"description\": \"Snapshots of targets at the time of release creation\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TargetSnapshot\"\n      }\n    },\n    \"renderState\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The current state of the render operation\",\n      \"enum\": [\"SUCCEEDED\", \"FAILED\", \"IN_PROGRESS\"]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which the release was created\"\n    },\n    \"renderStartTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which the render began\"\n    },\n    \"renderEndTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time at which the render completed\"\n    }\n  },\n  \"$defs\": {\n    \"BuildArtifact\": {\n      \"type\": \"object\",\n      \"description\": \"A build artifact with image and tag\",\n      \"properties\": {\n        \"image\": {\n          \"type\": \"string\",\n          \"description\": \"The container image name\"\n        },\n        \"tag\": {\n          \"type\": \"string\",\n          \"description\": \"The container image tag or digest\"\
  \n        }\n      }\n    },\n    \"DeliveryPipelineSnapshot\": {\n      \"type\": \"object\",\n      \"description\": \"Snapshot of a delivery pipeline\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"serialPipeline\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"stages\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"targetId\": {\n                    \"type\": \"string\"\n                  },\n                  \"profiles\": {\n                    \"type\": \"array\",\n                    \"items\": {\n                      \"type\": \"string\"\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"TargetSnapshot\": {\n      \"type\": \"object\",\n      \"description\": \"Snapshot of a deployment\
  \ target\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"targetId\": {\n          \"type\": \"string\"\n        },\n        \"requireApproval\": {\n          \"type\": \"boolean\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-deploy/refs/heads/main/json-schema/google-cloud-deploy-release-schema.json
tags:
- Continuous Delivery
- Deployment
- DevOps
- Kubernetes
- Pipeline
- Release Management
title: Google Cloud Deploy Release
---
