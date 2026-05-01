---
description: Defines a Dataflow job representing a pipeline execution. A job encapsulates the pipeline configuration, environment, execution state, and metadata for batch or streaming workloads on Google Cloud Platform.
layout: schema
name: Google Cloud Dataflow Job
properties_list:
- description: The unique identifier of the job, assigned by the server and immutable once set.
  name: id
  type: string
- description: The ID of the Google Cloud project that owns this job.
  name: projectId
  type: string
- description: The user-assigned name of the job. Job names do not need to be unique within a project.
  name: name
  type: string
- description: The type of Dataflow job, indicating batch or streaming execution.
  name: type
  type: string
- description: The current state of the job, representing its lifecycle position from creation through completion or cancellation.
  name: currentState
  type: string
- description: The timestamp of the most recent state transition.
  name: currentStateTime
  type: string
- description: The state requested for the job, such as cancelling or draining.
  name: requestedState
  type: string
- description: The timestamp when the job was initially created.
  name: createTime
  type: string
- description: The timestamp when the job began executing.
  name: startTime
  type: string
- description: The execution environment configuration for the job.
  name: environment
  type: object
- description: The pipeline processing steps that define the job.
  name: steps
  type: array
- description: The Cloud Storage location where step information is stored.
  name: stepsLocation
  type: string
- description: The per-stage execution state information for the job.
  name: stageStates
  type: array
- description: A description of the pipeline structure.
  name: pipelineDescription
  type: object
- description: User-defined labels for the job as key-value string pairs.
  name: labels
  type: object
- description: The regional endpoint where this job runs, such as us-central1.
  name: location
  type: string
- description: If this job was created from a snapshot, the ID of that snapshot.
  name: createdFromSnapshotId
  type: string
- description: If this job has been replaced by another job, the ID of the replacement.
  name: replacedByJobId
  type: string
- description: If this job is replacing another job, the ID of the job being replaced.
  name: replaceJobId
  type: string
- description: A unique client-generated idempotency key for preventing duplicate job creation.
  name: clientRequestId
  type: string
- description: A set of Cloud Storage files used for temporary storage.
  name: tempFiles
  type: array
- description: Metadata about the job for filtering and discovery.
  name: jobMetadata
  type: object
- description: Parameters that can be updated during execution without stopping the job.
  name: runtimeUpdatableParams
  type: object
- description: Resources allocated by the Dataflow service for the job.
  name: serviceResources
  type: object
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schema_file: json-schema/google-cloud-dataflow-job-schema.json
slug: google-cloud-dataflow-job
source_filename: google-cloud-dataflow-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/google-cloud-dataflow/json-schema/google-cloud-dataflow-job-schema.json\",\n  \"title\": \"Google Cloud Dataflow Job\",\n  \"description\": \"Defines a Dataflow job representing a pipeline execution. A job encapsulates the pipeline configuration, environment, execution state, and metadata for batch or streaming workloads on Google Cloud Platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the job, assigned by the server and immutable once set.\",\n      \"readOnly\": true\n    },\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the Google Cloud project that owns this job.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user-assigned name of the job. Job names do not need to be unique within\
  \ a project.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of Dataflow job, indicating batch or streaming execution.\",\n      \"enum\": [\n        \"JOB_TYPE_UNKNOWN\",\n        \"JOB_TYPE_BATCH\",\n        \"JOB_TYPE_STREAMING\"\n      ]\n    },\n    \"currentState\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the job, representing its lifecycle position from creation through completion or cancellation.\",\n      \"enum\": [\n        \"JOB_STATE_UNKNOWN\",\n        \"JOB_STATE_STOPPED\",\n        \"JOB_STATE_RUNNING\",\n        \"JOB_STATE_DONE\",\n        \"JOB_STATE_FAILED\",\n        \"JOB_STATE_CANCELLED\",\n        \"JOB_STATE_UPDATED\",\n        \"JOB_STATE_DRAINING\",\n        \"JOB_STATE_DRAINED\",\n        \"JOB_STATE_PENDING\",\n        \"JOB_STATE_CANCELLING\",\n        \"JOB_STATE_QUEUED\",\n        \"JOB_STATE_RESOURCE_CLEANING_UP\"\n      ],\n      \"readOnly\": true\n    },\n    \"currentStateTime\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of the most recent state transition.\",\n      \"readOnly\": true\n    },\n    \"requestedState\": {\n      \"type\": \"string\",\n      \"description\": \"The state requested for the job, such as cancelling or draining.\",\n      \"enum\": [\n        \"JOB_STATE_UNKNOWN\",\n        \"JOB_STATE_STOPPED\",\n        \"JOB_STATE_RUNNING\",\n        \"JOB_STATE_DONE\",\n        \"JOB_STATE_FAILED\",\n        \"JOB_STATE_CANCELLED\",\n        \"JOB_STATE_UPDATED\",\n        \"JOB_STATE_DRAINING\",\n        \"JOB_STATE_DRAINED\",\n        \"JOB_STATE_PENDING\",\n        \"JOB_STATE_CANCELLING\",\n        \"JOB_STATE_QUEUED\",\n        \"JOB_STATE_RESOURCE_CLEANING_UP\"\n      ]\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the job was initially created.\",\n      \"readOnly\": true\n    },\n   \
  \ \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the job began executing.\",\n      \"readOnly\": true\n    },\n    \"environment\": {\n      \"$ref\": \"google-cloud-dataflow-environment-schema.json\",\n      \"description\": \"The execution environment configuration for the job.\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"The pipeline processing steps that define the job.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"kind\": {\n            \"type\": \"string\",\n            \"description\": \"The type of transform this step represents.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The unique name of this step within the job.\"\n          },\n          \"properties\": {\n            \"type\": \"object\",\n            \"description\": \"Named properties associated with\
  \ the step.\",\n            \"additionalProperties\": true\n          }\n        }\n      }\n    },\n    \"stepsLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The Cloud Storage location where step information is stored.\"\n    },\n    \"stageStates\": {\n      \"type\": \"array\",\n      \"description\": \"The per-stage execution state information for the job.\",\n      \"readOnly\": true,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"executionStageName\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the execution stage.\"\n          },\n          \"executionStageState\": {\n            \"type\": \"string\",\n            \"description\": \"The state of the execution stage.\",\n            \"enum\": [\n              \"JOB_STATE_UNKNOWN\",\n              \"JOB_STATE_STOPPED\",\n              \"JOB_STATE_RUNNING\",\n              \"JOB_STATE_DONE\",\n              \"JOB_STATE_FAILED\",\n\
  \              \"JOB_STATE_CANCELLED\",\n              \"JOB_STATE_UPDATED\",\n              \"JOB_STATE_DRAINING\",\n              \"JOB_STATE_DRAINED\",\n              \"JOB_STATE_PENDING\",\n              \"JOB_STATE_CANCELLING\",\n              \"JOB_STATE_QUEUED\",\n              \"JOB_STATE_RESOURCE_CLEANING_UP\"\n            ]\n          },\n          \"currentStateTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The time at which the stage entered its current state.\"\n          }\n        }\n      }\n    },\n    \"pipelineDescription\": {\n      \"$ref\": \"google-cloud-dataflow-pipeline-schema.json\",\n      \"description\": \"A description of the pipeline structure.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"User-defined labels for the job as key-value string pairs.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"location\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The regional endpoint where this job runs, such as us-central1.\"\n    },\n    \"createdFromSnapshotId\": {\n      \"type\": \"string\",\n      \"description\": \"If this job was created from a snapshot, the ID of that snapshot.\",\n      \"readOnly\": true\n    },\n    \"replacedByJobId\": {\n      \"type\": \"string\",\n      \"description\": \"If this job has been replaced by another job, the ID of the replacement.\",\n      \"readOnly\": true\n    },\n    \"replaceJobId\": {\n      \"type\": \"string\",\n      \"description\": \"If this job is replacing another job, the ID of the job being replaced.\"\n    },\n    \"clientRequestId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique client-generated idempotency key for preventing duplicate job creation.\"\n    },\n    \"tempFiles\": {\n      \"type\": \"array\",\n      \"description\": \"A set of Cloud Storage files used for temporary storage.\",\n      \"\
  items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jobMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the job for filtering and discovery.\",\n      \"properties\": {\n        \"sdkVersion\": {\n          \"type\": \"object\",\n          \"description\": \"The version of the SDK used to run the job.\",\n          \"properties\": {\n            \"version\": {\n              \"type\": \"string\",\n              \"description\": \"The version string.\"\n            },\n            \"versionDisplayName\": {\n              \"type\": \"string\",\n              \"description\": \"A human-readable version name.\"\n            },\n            \"sdkSupportStatus\": {\n              \"type\": \"string\",\n              \"description\": \"The support status for this SDK version.\",\n              \"enum\": [\"UNKNOWN\", \"SUPPORTED\", \"STALE\", \"DEPRECATED\", \"UNSUPPORTED\"]\n            }\n          }\n        },\n        \"spannerDetails\": {\n\
  \          \"type\": \"array\",\n          \"description\": \"Cloud Spanner sources used by this job.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"projectId\": { \"type\": \"string\" },\n              \"instanceId\": { \"type\": \"string\" },\n              \"databaseId\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"bigqueryDetails\": {\n          \"type\": \"array\",\n          \"description\": \"BigQuery sources used by this job.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"table\": { \"type\": \"string\" },\n              \"dataset\": { \"type\": \"string\" },\n              \"projectId\": { \"type\": \"string\" },\n              \"query\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"bigTableDetails\": {\n          \"type\": \"array\",\n          \"description\": \"Cloud Bigtable sources used\
  \ by this job.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"projectId\": { \"type\": \"string\" },\n              \"instanceId\": { \"type\": \"string\" },\n              \"tableId\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"pubsubDetails\": {\n          \"type\": \"array\",\n          \"description\": \"Pub/Sub sources used by this job.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"topic\": { \"type\": \"string\" },\n              \"subscription\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"fileDetails\": {\n          \"type\": \"array\",\n          \"description\": \"File-based sources used by this job.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"filePattern\": { \"type\": \"string\" }\n            }\n          }\n        },\n\
  \        \"datastoreDetails\": {\n          \"type\": \"array\",\n          \"description\": \"Datastore sources used by this job.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"namespace\": { \"type\": \"string\" },\n              \"projectId\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"userDisplayProperties\": {\n          \"type\": \"object\",\n          \"description\": \"User-supplied properties for display.\",\n          \"additionalProperties\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"runtimeUpdatableParams\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters that can be updated during execution without stopping the job.\",\n      \"properties\": {\n        \"maxNumWorkers\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"description\": \"The maximum number of workers for autoscaling.\"\n        },\n        \"\
  minNumWorkers\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"description\": \"The minimum number of workers for autoscaling.\"\n        },\n        \"workerUtilizationHint\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Target worker utilization between 0.1 and 0.9.\"\n        }\n      }\n    },\n    \"serviceResources\": {\n      \"type\": \"object\",\n      \"description\": \"Resources allocated by the Dataflow service for the job.\",\n      \"properties\": {\n        \"zones\": {\n          \"type\": \"array\",\n          \"description\": \"The Cloud zones from which resources are allocated.\",\n          \"items\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/json-schema/google-cloud-dataflow-job-schema.json
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
title: Google Cloud Dataflow Job
---
