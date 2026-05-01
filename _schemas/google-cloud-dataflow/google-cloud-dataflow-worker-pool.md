---
description: Describes a pool of workers that execute pipeline transforms, including machine type, disk configuration, networking, and autoscaling behavior.
layout: schema
name: Google Cloud Dataflow Worker Pool
properties_list:
- description: The kind of worker pool, either harness for pipeline execution or shuffle for shuffle operations.
  name: kind
  type: string
- description: The initial number of worker instances in the pool.
  name: numWorkers
  type: integer
- description: The Compute Engine machine type for worker instances, such as n1-standard-4 or e2-standard-2.
  name: machineType
  type: string
- description: The size in GB of the root disk for each worker instance.
  name: diskSizeGb
  type: integer
- description: The type of root disk for each worker instance, such as pd-standard, pd-ssd, or pd-balanced.
  name: diskType
  type: string
- description: The Compute Engine zone where worker instances should be created.
  name: zone
  type: string
- description: The name or full URL of the VPC network for worker instances.
  name: network
  type: string
- description: The full URL of the VPC subnetwork for worker instances.
  name: subnetwork
  type: string
- description: Metadata key-value pairs to set on the worker Compute Engine instances.
  name: metadata
  type: object
- description: Packages to install on each worker instance.
  name: packages
  type: array
- description: The default package set to install on the worker instances.
  name: defaultPackageSet
  type: string
- description: Settings for autoscaling the number of worker instances in a pool.
  name: autoscalingSettings
  type: object
- description: Configuration for the network IP address assignment for workers.
  name: ipConfiguration
  type: string
- description: Set of SDK harness container images for the worker pool.
  name: sdkHarnessContainerImages
  type: array
- description: The policy that determines when worker instances are torn down.
  name: teardownPolicy
  type: string
- description: The Docker container image to use for the worker harness.
  name: workerHarnessContainerImage
  type: string
provider_name: Google Cloud Dataflow
provider_slug: google-cloud-dataflow
schema_file: json-schema/google-cloud-dataflow-worker-pool-schema.json
slug: google-cloud-dataflow-worker-pool
source_filename: google-cloud-dataflow-worker-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/google-cloud-dataflow/json-schema/google-cloud-dataflow-worker-pool-schema.json\",\n  \"title\": \"Google Cloud Dataflow Worker Pool\",\n  \"description\": \"Describes a pool of workers that execute pipeline transforms, including machine type, disk configuration, networking, and autoscaling behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"The kind of worker pool, either harness for pipeline execution or shuffle for shuffle operations.\"\n    },\n    \"numWorkers\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"The initial number of worker instances in the pool.\"\n    },\n    \"machineType\": {\n      \"type\": \"string\",\n      \"description\": \"The Compute Engine machine type for worker instances, such as n1-standard-4 or e2-standard-2.\"\
  \n    },\n    \"diskSizeGb\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\",\n      \"description\": \"The size in GB of the root disk for each worker instance.\"\n    },\n    \"diskType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of root disk for each worker instance, such as pd-standard, pd-ssd, or pd-balanced.\"\n    },\n    \"zone\": {\n      \"type\": \"string\",\n      \"description\": \"The Compute Engine zone where worker instances should be created.\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"The name or full URL of the VPC network for worker instances.\"\n    },\n    \"subnetwork\": {\n      \"type\": \"string\",\n      \"description\": \"The full URL of the VPC subnetwork for worker instances.\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata key-value pairs to set on the worker Compute Engine instances.\",\n      \"additionalProperties\": {\n       \
  \ \"type\": \"string\"\n      }\n    },\n    \"packages\": {\n      \"type\": \"array\",\n      \"description\": \"Packages to install on each worker instance.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the package.\"\n          },\n          \"location\": {\n            \"type\": \"string\",\n            \"description\": \"The Cloud Storage location of the package.\"\n          }\n        }\n      }\n    },\n    \"defaultPackageSet\": {\n      \"type\": \"string\",\n      \"description\": \"The default package set to install on the worker instances.\",\n      \"enum\": [\n        \"DEFAULT_PACKAGE_SET_UNKNOWN\",\n        \"DEFAULT_PACKAGE_SET_NONE\",\n        \"DEFAULT_PACKAGE_SET_JAVA\",\n        \"DEFAULT_PACKAGE_SET_PYTHON\"\n      ]\n    },\n    \"autoscalingSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Settings for autoscaling\
  \ the number of worker instances in a pool.\",\n      \"properties\": {\n        \"algorithm\": {\n          \"type\": \"string\",\n          \"description\": \"The autoscaling algorithm to use.\",\n          \"enum\": [\n            \"AUTOSCALING_ALGORITHM_UNKNOWN\",\n            \"AUTOSCALING_ALGORITHM_NONE\",\n            \"AUTOSCALING_ALGORITHM_BASIC\"\n          ]\n        },\n        \"maxNumWorkers\": {\n          \"type\": \"integer\",\n          \"format\": \"int32\",\n          \"description\": \"The maximum number of workers to scale up to.\"\n        }\n      }\n    },\n    \"ipConfiguration\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration for the network IP address assignment for workers.\",\n      \"enum\": [\n        \"WORKER_IP_UNSPECIFIED\",\n        \"WORKER_IP_PUBLIC\",\n        \"WORKER_IP_PRIVATE\"\n      ]\n    },\n    \"sdkHarnessContainerImages\": {\n      \"type\": \"array\",\n      \"description\": \"Set of SDK harness container images\
  \ for the worker pool.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"containerImage\": {\n            \"type\": \"string\",\n            \"description\": \"The Docker container image URI.\"\n          },\n          \"useSingleCorePerContainer\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether to use a single CPU core per container.\"\n          },\n          \"environmentId\": {\n            \"type\": \"string\",\n            \"description\": \"The environment ID this container image is associated with.\"\n          },\n          \"capabilities\": {\n            \"type\": \"array\",\n            \"description\": \"The capabilities of this SDK harness container.\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"teardownPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"The policy that determines when worker instances\
  \ are torn down.\",\n      \"enum\": [\n        \"TEARDOWN_POLICY_UNKNOWN\",\n        \"TEARDOWN_ALWAYS\",\n        \"TEARDOWN_ON_SUCCESS\",\n        \"TEARDOWN_NEVER\"\n      ]\n    },\n    \"workerHarnessContainerImage\": {\n      \"type\": \"string\",\n      \"description\": \"The Docker container image to use for the worker harness.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-dataflow/refs/heads/main/json-schema/google-cloud-dataflow-worker-pool-schema.json
tags:
- Apache Beam
- Batch Processing
- Big Data
- Data Processing
- ETL
- Stream Processing
title: Google Cloud Dataflow Worker Pool
---
