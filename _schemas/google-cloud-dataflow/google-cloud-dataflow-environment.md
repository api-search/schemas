---
description: Describes the environment in which a Dataflow job runs, including worker pool configuration, networking, encryption, and runtime settings.
layout: schema
name: Google Cloud Dataflow Environment
properties_list:
- description: The prefix of the Cloud Storage path for temporary storage used during job execution.
  name: tempStoragePrefix
  type: string
- description: The type of cluster manager API to use for managing workers.
  name: clusterManagerApiService
  type: string
- description: A list of experiment flags passed to the SDK and Dataflow service for enabling experimental features.
  name: experiments
  type: array
- description: A list of service-level feature flags for the Dataflow service.
  name: serviceOptions
  type: array
- description: 'The Cloud KMS key used for encrypting data at rest. Format: projects/{project}/locations/{location}/keyRings/{keyRing}/cryptoKeys/{key}.'
  name: serviceKmsKeyName
  type: string
- description: The worker pool configuration for the job, defining machine type, disk, network, and autoscaling settings.
  name: workerPools
  type: array
- description: A structure describing the SDK and its version used by the job.
  name: userAgent
  type: object
- description: A structure describing which version of the Dataflow service the job requires.
  name: version
  type: object
- description: 'The BigQuery dataset for workflow logging tables. Format: bigquery.googleapis.com/projects/{project}/datasets/{dataset}.'
  name: dataset
  type: string
- description: The Cloud Dataflow SDK pipeline options specified by the user.
  name: sdkPipelineOptions
  type: object
- description: The email address of the service account to run the workers as.
  name: serviceAccountEmail
  type: string
- description: Which Flexible Resource Scheduling mode to run in for Flex RS jobs.
  name: flexResourceSchedulingGoal
  type: string
- description: The Compute Engine region where workers should be created.
  name: workerRegion
  type: string
- description: The specific Compute Engine zone where workers should be created.
  name: workerZone
  type: string
- description: The shuffle mode for the job, set by the service.
  name: shuffleMode
  type: string
- description: Debugging options for the job.
  name: debugOptions
  type: object
- description: The streaming mode for the job, specifying the message processing guarantee.
  name: streamingMode
  type: string
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schema_file: json-schema/google-cloud-dataflow-environment-schema.json
slug: google-cloud-dataflow-environment
source_filename: google-cloud-dataflow-environment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/google-cloud-dataflow/json-schema/google-cloud-dataflow-environment-schema.json\",\n  \"title\": \"Google Cloud Dataflow Environment\",\n  \"description\": \"Describes the environment in which a Dataflow job runs, including worker pool configuration, networking, encryption, and runtime settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tempStoragePrefix\": {\n      \"type\": \"string\",\n      \"description\": \"The prefix of the Cloud Storage path for temporary storage used during job execution.\"\n    },\n    \"clusterManagerApiService\": {\n      \"type\": \"string\",\n      \"description\": \"The type of cluster manager API to use for managing workers.\"\n    },\n    \"experiments\": {\n      \"type\": \"array\",\n      \"description\": \"A list of experiment flags passed to the SDK and Dataflow service for enabling experimental features.\",\n \
  \     \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"serviceOptions\": {\n      \"type\": \"array\",\n      \"description\": \"A list of service-level feature flags for the Dataflow service.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"serviceKmsKeyName\": {\n      \"type\": \"string\",\n      \"description\": \"The Cloud KMS key used for encrypting data at rest. Format: projects/{project}/locations/{location}/keyRings/{keyRing}/cryptoKeys/{key}.\"\n    },\n    \"workerPools\": {\n      \"type\": \"array\",\n      \"description\": \"The worker pool configuration for the job, defining machine type, disk, network, and autoscaling settings.\",\n      \"items\": {\n        \"$ref\": \"google-cloud-dataflow-worker-pool-schema.json\"\n      }\n    },\n    \"userAgent\": {\n      \"type\": \"object\",\n      \"description\": \"A structure describing the SDK and its version used by the job.\",\n      \"additionalProperties\": true\n    },\n \
  \   \"version\": {\n      \"type\": \"object\",\n      \"description\": \"A structure describing which version of the Dataflow service the job requires.\",\n      \"additionalProperties\": true\n    },\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"The BigQuery dataset for workflow logging tables. Format: bigquery.googleapis.com/projects/{project}/datasets/{dataset}.\"\n    },\n    \"sdkPipelineOptions\": {\n      \"type\": \"object\",\n      \"description\": \"The Cloud Dataflow SDK pipeline options specified by the user.\",\n      \"additionalProperties\": true\n    },\n    \"serviceAccountEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the service account to run the workers as.\"\n    },\n    \"flexResourceSchedulingGoal\": {\n      \"type\": \"string\",\n      \"description\": \"Which Flexible Resource Scheduling mode to run in for Flex RS jobs.\",\n      \"enum\": [\n        \"FLEXRS_UNSPECIFIED\"\
  ,\n        \"FLEXRS_SPEED_OPTIMIZED\",\n        \"FLEXRS_COST_OPTIMIZED\"\n      ]\n    },\n    \"workerRegion\": {\n      \"type\": \"string\",\n      \"description\": \"The Compute Engine region where workers should be created.\"\n    },\n    \"workerZone\": {\n      \"type\": \"string\",\n      \"description\": \"The specific Compute Engine zone where workers should be created.\"\n    },\n    \"shuffleMode\": {\n      \"type\": \"string\",\n      \"description\": \"The shuffle mode for the job, set by the service.\",\n      \"readOnly\": true,\n      \"enum\": [\n        \"SHUFFLE_MODE_UNSPECIFIED\",\n        \"VM_BASED\",\n        \"SERVICE_BASED\"\n      ]\n    },\n    \"debugOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Debugging options for the job.\",\n      \"properties\": {\n        \"enableHotKeyLogging\": {\n          \"type\": \"boolean\",\n          \"description\": \"When true, enables logging of hot key detections during job execution.\"\n        }\n\
  \      }\n    },\n    \"streamingMode\": {\n      \"type\": \"string\",\n      \"description\": \"The streaming mode for the job, specifying the message processing guarantee.\",\n      \"enum\": [\n        \"STREAMING_MODE_UNSPECIFIED\",\n        \"STREAMING_MODE_EXACTLY_ONCE\",\n        \"STREAMING_MODE_AT_LEAST_ONCE\"\n      ]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/json-schema/google-cloud-dataflow-environment-schema.json
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
title: Google Cloud Dataflow Environment
---
