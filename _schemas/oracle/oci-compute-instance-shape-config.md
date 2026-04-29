---
description: The shape configuration for an instance. This includes the number of OCPUs, amount of memory, and networking bandwidth.
layout: schema
name: InstanceShapeConfig
properties_list:
- description: The total number of OCPUs available to the instance
  name: ocpus
  type: number
- description: The total amount of memory available to the instance, in gigabytes
  name: memoryInGBs
  type: number
- description: The baseline OCPU utilization for a subcore burstable instance
  name: baselineOcpuUtilization
  type: string
- description: A short description of the instance processor
  name: processorDescription
  type: string
- description: The networking bandwidth available to the instance, in Gbps
  name: networkingBandwidthInGbps
  type: number
- description: The maximum number of VNIC attachments for the instance
  name: maxVnicAttachments
  type: integer
- description: The number of GPUs available to the instance
  name: gpus
  type: integer
- description: A short description of the instance GPU
  name: gpuDescription
  type: string
- description: The number of local disks available to the instance
  name: localDisks
  type: integer
- description: The aggregate size of all local disks, in gigabytes
  name: localDisksTotalSizeInGBs
  type: number
- description: The total number of VCPUs available to the instance. This is typically 2x the number of OCPUs.
  name: vcpus
  type: integer
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-instance-shape-config-schema.json
slug: oci-compute-instance-shape-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InstanceShapeConfig\",\n  \"type\": \"object\",\n  \"description\": \"The shape configuration for an instance. This includes the number of OCPUs, amount of memory, and networking bandwidth.\",\n  \"properties\": {\n    \"ocpus\": {\n      \"type\": \"number\",\n      \"description\": \"The total number of OCPUs available to the instance\"\n    },\n    \"memoryInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount of memory available to the instance, in gigabytes\"\n    },\n    \"baselineOcpuUtilization\": {\n      \"type\": \"string\",\n      \"description\": \"The baseline OCPU utilization for a subcore burstable instance\"\n    },\n    \"processorDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the instance processor\"\n    },\n    \"networkingBandwidthInGbps\": {\n      \"type\": \"number\",\n      \"description\":\
  \ \"The networking bandwidth available to the instance, in Gbps\"\n    },\n    \"maxVnicAttachments\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of VNIC attachments for the instance\"\n    },\n    \"gpus\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of GPUs available to the instance\"\n    },\n    \"gpuDescription\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the instance GPU\"\n    },\n    \"localDisks\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of local disks available to the instance\"\n    },\n    \"localDisksTotalSizeInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The aggregate size of all local disks, in gigabytes\"\n    },\n    \"vcpus\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of VCPUs available to the instance. This is typically 2x the number of OCPUs.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-instance-shape-config-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: InstanceShapeConfig
---
