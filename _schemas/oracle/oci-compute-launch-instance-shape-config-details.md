---
description: The shape configuration details for launching a flexible instance. Required when using a flexible shape (e.g., VM.Standard.E4.Flex).
layout: schema
name: LaunchInstanceShapeConfigDetails
properties_list:
- description: The total number of OCPUs available to the instance. For flexible shapes, specify the desired number of OCPUs.
  name: ocpus
  type: number
- description: The total amount of memory in gigabytes. For flexible shapes, the amount of memory per OCPU can vary. The default ratio is typically 1 OCPU to 16 GB of memory.
  name: memoryInGBs
  type: number
- description: The baseline OCPU utilization for a subcore burstable instance. Leave unset for a non-burstable instance or to use the default baseline.
  name: baselineOcpuUtilization
  type: string
- description: The number of NVMe drives to attach to the instance
  name: nvmes
  type: integer
provider_name: Oracle
provider_slug: oracle
schema_file: json-schema/oci-compute-launch-instance-shape-config-details-schema.json
slug: oci-compute-launch-instance-shape-config-details
source_filename: oci-compute-launch-instance-shape-config-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LaunchInstanceShapeConfigDetails\",\n  \"type\": \"object\",\n  \"description\": \"The shape configuration details for launching a flexible instance. Required when using a flexible shape (e.g., VM.Standard.E4.Flex).\",\n  \"properties\": {\n    \"ocpus\": {\n      \"type\": \"number\",\n      \"description\": \"The total number of OCPUs available to the instance. For flexible shapes, specify the desired number of OCPUs.\"\n    },\n    \"memoryInGBs\": {\n      \"type\": \"number\",\n      \"description\": \"The total amount of memory in gigabytes. For flexible shapes, the amount of memory per OCPU can vary. The default ratio is typically 1 OCPU to 16 GB of memory.\"\n    },\n    \"baselineOcpuUtilization\": {\n      \"type\": \"string\",\n      \"description\": \"The baseline OCPU utilization for a subcore burstable instance. Leave unset for a non-burstable instance or to use the default baseline.\"\
  \n    },\n    \"nvmes\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of NVMe drives to attach to the instance\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle/refs/heads/main/json-schema/oci-compute-launch-instance-shape-config-details-schema.json
tags:
- Cloud
- Database
- Enterprise
- Infrastructure
- SaaS
title: LaunchInstanceShapeConfigDetails
---
