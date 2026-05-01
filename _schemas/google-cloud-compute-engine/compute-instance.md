---
description: Represents a Compute Engine virtual machine instance resource, including its machine type, disks, network interfaces, and status.
layout: schema
name: Google Compute Engine Instance
properties_list:
- description: The unique identifier for the resource.
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: An optional description of the resource.
  name: description
  type: string
- description: URL of the zone where the instance resides.
  name: zone
  type: string
- description: Full or partial URL of the machine type resource to use for this instance.
  name: machineType
  type: string
- description: The status of the instance.
  name: status
  type: string
- description: An array of network configurations for this instance.
  name: networkInterfaces
  type: array
- description: Array of disks associated with this instance.
  name: disks
  type: array
- description: Server-defined URL for this resource.
  name: selfLink
  type: string
- description: Creation timestamp in RFC3339 text format.
  name: creationTimestamp
  type: string
provider_name: Google Cloud Compute Engine
provider_slug: google-cloud-compute-engine
schema_file: json-schema/compute-instance.json
slug: compute-instance
source_filename: compute-instance.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-compute-engine/refs/heads/main/json-schema/compute-instance.json\",\n  \"title\": \"Google Compute Engine Instance\",\n  \"description\": \"Represents a Compute Engine virtual machine instance resource, including its machine type, disks, network interfaces, and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the resource.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"An optional description of the resource.\"\n    },\n    \"zone\": {\n      \"type\": \"string\",\n      \"description\": \"URL of the zone where the instance resides.\"\n    },\n    \"machineType\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Full or partial URL of the machine type resource to use for this instance.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the instance.\",\n      \"enum\": [\n        \"PROVISIONING\",\n        \"STAGING\",\n        \"RUNNING\",\n        \"STOPPING\",\n        \"STOPPED\",\n        \"SUSPENDING\",\n        \"SUSPENDED\",\n        \"TERMINATED\"\n      ]\n    },\n    \"networkInterfaces\": {\n      \"type\": \"array\",\n      \"description\": \"An array of network configurations for this instance.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"network\": {\n            \"type\": \"string\"\n          },\n          \"subnetwork\": {\n            \"type\": \"string\"\n          },\n          \"networkIP\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"disks\": {\n      \"type\": \"array\",\n      \"description\": \"Array of disks\
  \ associated with this instance.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"source\": {\n            \"type\": \"string\"\n          },\n          \"boot\": {\n            \"type\": \"boolean\"\n          },\n          \"autoDelete\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    },\n    \"selfLink\": {\n      \"type\": \"string\",\n      \"description\": \"Server-defined URL for this resource.\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation timestamp in RFC3339 text format.\"\n    }\n  },\n  \"required\": [\"name\", \"machineType\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-compute-engine/refs/heads/main/json-schema/compute-instance.json
tags:
- Compute
- Google Cloud
- IaaS
- Infrastructure
- Virtual Machines
title: Google Compute Engine Instance
---
