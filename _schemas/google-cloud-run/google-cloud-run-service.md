---
description: Represents a Cloud Run service, which is a serverless application that runs stateless containers invocable via HTTP requests.
layout: schema
name: Google Cloud Run Service
properties_list:
- description: The fully qualified name of the service in the format projects/{project}/locations/{location}/services/{service}.
  name: name
  type: string
- description: User-provided description of the service.
  name: description
  type: string
- description: Output only. Server-assigned unique identifier for the service.
  name: uid
  type: string
- description: Output only. A number that monotonically increases every time the user modifies the service.
  name: generation
  type: string
- description: Unstructured key-value map for user-defined labels.
  name: labels
  type: object
- description: Unstructured key-value map for user-defined annotations.
  name: annotations
  type: object
- description: Output only. The creation time.
  name: createTime
  type: string
- description: Output only. The last-modified time.
  name: updateTime
  type: string
- description: Provides the ingress settings for this service.
  name: ingress
  type: string
- description: The launch stage as defined by Google Cloud Platform Launch Stages.
  name: launchStage
  type: string
- description: The template used to create revisions for this service.
  name: template
  type: object
- description: Specifies how to distribute traffic over a collection of revisions.
  name: traffic
  type: array
- description: Output only. The main URI where the service is serving traffic.
  name: uri
  type: string
- description: Output only. Name of the latest revision that is serving traffic.
  name: latestReadyRevision
  type: string
- description: Output only. Name of the last created revision.
  name: latestCreatedRevision
  type: string
provider_name: Google Cloud Run
provider_slug: google-cloud-run
schema_file: json-schema/google-cloud-run-service-schema.json
slug: google-cloud-run-service
source_filename: google-cloud-run-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-run/refs/heads/main/json-schema/google-cloud-run-service-schema.json\",\n  \"title\": \"Google Cloud Run Service\",\n  \"description\": \"Represents a Cloud Run service, which is a serverless application that runs stateless containers invocable via HTTP requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The fully qualified name of the service in the format projects/{project}/locations/{location}/services/{service}.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-provided description of the service.\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Server-assigned unique identifier for the service.\"\n    },\n    \"generation\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Output only. A number that monotonically increases every time the user modifies the service.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"string\" },\n      \"description\": \"Unstructured key-value map for user-defined labels.\"\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"string\" },\n      \"description\": \"Unstructured key-value map for user-defined annotations.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The creation time.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Output only. The last-modified time.\"\n    },\n    \"ingress\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"INGRESS_TRAFFIC_UNSPECIFIED\",\n        \"INGRESS_TRAFFIC_ALL\",\n        \"INGRESS_TRAFFIC_INTERNAL_ONLY\"\
  ,\n        \"INGRESS_TRAFFIC_INTERNAL_LOAD_BALANCER\"\n      ],\n      \"description\": \"Provides the ingress settings for this service.\"\n    },\n    \"launchStage\": {\n      \"type\": \"string\",\n      \"enum\": [\"LAUNCH_STAGE_UNSPECIFIED\", \"UNIMPLEMENTED\", \"PRELAUNCH\", \"EARLY_ACCESS\", \"ALPHA\", \"BETA\", \"GA\", \"DEPRECATED\"],\n      \"description\": \"The launch stage as defined by Google Cloud Platform Launch Stages.\"\n    },\n    \"template\": {\n      \"type\": \"object\",\n      \"description\": \"The template used to create revisions for this service.\",\n      \"properties\": {\n        \"revision\": { \"type\": \"string\" },\n        \"scaling\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"minInstanceCount\": { \"type\": \"integer\" },\n            \"maxInstanceCount\": { \"type\": \"integer\" }\n          }\n        },\n        \"timeout\": { \"type\": \"string\" },\n        \"serviceAccount\": { \"type\": \"string\" },\n \
  \       \"containers\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"image\": { \"type\": \"string\", \"description\": \"Container image URI.\" },\n              \"command\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"args\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"env\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": { \"type\": \"string\" },\n                    \"value\": { \"type\": \"string\" }\n                  }\n                }\n              },\n              \"resources\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"limits\": {\n                    \"type\": \"object\",\n \
  \                   \"additionalProperties\": { \"type\": \"string\" }\n                  },\n                  \"cpuIdle\": { \"type\": \"boolean\" },\n                  \"startupCpuBoost\": { \"type\": \"boolean\" }\n                }\n              },\n              \"ports\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": { \"type\": \"string\" },\n                    \"containerPort\": { \"type\": \"integer\" }\n                  }\n                }\n              }\n            },\n            \"required\": [\"image\"]\n          }\n        },\n        \"maxInstanceRequestConcurrency\": { \"type\": \"integer\" },\n        \"executionEnvironment\": {\n          \"type\": \"string\",\n          \"enum\": [\"EXECUTION_ENVIRONMENT_UNSPECIFIED\", \"EXECUTION_ENVIRONMENT_GEN1\", \"EXECUTION_ENVIRONMENT_GEN2\"]\n        }\n      }\n    },\n    \"traffic\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Specifies how to distribute traffic over a collection of revisions.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\"TRAFFIC_TARGET_ALLOCATION_TYPE_UNSPECIFIED\", \"TRAFFIC_TARGET_ALLOCATION_TYPE_LATEST\", \"TRAFFIC_TARGET_ALLOCATION_TYPE_REVISION\"]\n          },\n          \"revision\": { \"type\": \"string\" },\n          \"percent\": { \"type\": \"integer\" },\n          \"tag\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Output only. The main URI where the service is serving traffic.\"\n    },\n    \"latestReadyRevision\": {\n      \"type\": \"string\",\n      \"description\": \"Output only. Name of the latest revision that is serving traffic.\"\n    },\n    \"latestCreatedRevision\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Output only. Name of the last created revision.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-run/refs/heads/main/json-schema/google-cloud-run-service-schema.json
tags:
- Cloud Run
- Containers
- Google Cloud
- Serverless
title: Google Cloud Run Service
---
