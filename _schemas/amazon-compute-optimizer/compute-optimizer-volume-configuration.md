---
description: Describes the configuration of an Amazon Elastic Block Store (Amazon EBS) volume.
layout: schema
name: VolumeConfiguration
properties_list:
- description: ''
  name: volumeType
  type: object
- description: ''
  name: volumeSize
  type: object
- description: ''
  name: volumeBaselineIOPS
  type: object
- description: ''
  name: volumeBurstIOPS
  type: object
- description: ''
  name: volumeBaselineThroughput
  type: object
- description: ''
  name: volumeBurstThroughput
  type: object
- description: ''
  name: rootVolume
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-volume-configuration-schema.json
slug: compute-optimizer-volume-configuration
source_filename: compute-optimizer-volume-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-volume-configuration-schema.json\",\n  \"title\": \"VolumeConfiguration\",\n  \"description\": \"Describes the configuration of an Amazon Elastic Block Store (Amazon EBS) volume.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"volumeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeType\"\n        },\n        {\n          \"description\": \"<p>The volume type.</p> <p>This can be <code>gp2</code> for General Purpose SSD, <code>io1</code> or <code>io2</code> for Provisioned IOPS SSD, <code>st1</code> for Throughput Optimized HDD, <code>sc1</code> for Cold HDD, or <code>standard</code> for Magnetic volumes.</p>\"\n        }\n      ]\n    },\n    \"volumeSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeSize\"\
  \n        },\n        {\n          \"description\": \"The size of the volume, in GiB.\"\n        }\n      ]\n    },\n    \"volumeBaselineIOPS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeBaselineIOPS\"\n        },\n        {\n          \"description\": \"The baseline IOPS of the volume.\"\n        }\n      ]\n    },\n    \"volumeBurstIOPS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeBurstIOPS\"\n        },\n        {\n          \"description\": \"The burst IOPS of the volume.\"\n        }\n      ]\n    },\n    \"volumeBaselineThroughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeBaselineThroughput\"\n        },\n        {\n          \"description\": \"The baseline throughput of the volume.\"\n        }\n      ]\n    },\n    \"volumeBurstThroughput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VolumeBurstThroughput\"\n        },\n\
  \        {\n          \"description\": \"The burst throughput of the volume.\"\n        }\n      ]\n    },\n    \"rootVolume\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RootVolume\"\n        },\n        {\n          \"description\": \" Contains the image used to boot the instance during launch. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-volume-configuration-schema.json
tags:
- AWS
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: VolumeConfiguration
---
