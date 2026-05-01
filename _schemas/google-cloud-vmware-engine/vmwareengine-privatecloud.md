---
description: Represents a VMware Engine private cloud resource, including its configuration, state, network settings, and management cluster.
layout: schema
name: Google Cloud VMware Engine Private Cloud
properties_list:
- description: The resource name of this private cloud.
  name: name
  type: string
- description: User-provided description for this private cloud.
  name: description
  type: string
- description: State of the resource.
  name: state
  type: string
- description: Network configuration for the private cloud.
  name: networkConfig
  type: object
- description: The management cluster for this private cloud.
  name: managementCluster
  type: object
- description: Creation time of the resource.
  name: createTime
  type: string
- description: Last update time of the resource.
  name: updateTime
  type: string
- description: Time when the resource will be irreversibly purged.
  name: expireTime
  type: string
provider_name: Google Cloud VMware Engine
provider_slug: google-cloud-vmware-engine
schema_file: json-schema/vmwareengine-privatecloud.json
slug: vmwareengine-privatecloud
source_filename: vmwareengine-privatecloud.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-search/google-cloud-vmware-engine/refs/heads/main/json-schema/vmwareengine-privatecloud.json\",\n  \"title\": \"Google Cloud VMware Engine Private Cloud\",\n  \"description\": \"Represents a VMware Engine private cloud resource, including its configuration, state, network settings, and management cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of this private cloud.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"User-provided description for this private cloud.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State of the resource.\",\n      \"enum\": [\n        \"STATE_UNSPECIFIED\",\n        \"ACTIVE\",\n        \"CREATING\",\n        \"UPDATING\",\n        \"FAILED\",\n        \"\
  DELETED\",\n        \"PURGING\"\n      ]\n    },\n    \"networkConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Network configuration for the private cloud.\",\n      \"properties\": {\n        \"managementCidr\": {\n          \"type\": \"string\",\n          \"description\": \"Management CIDR used by VMware management appliances.\"\n        },\n        \"vmwareEngineNetwork\": {\n          \"type\": \"string\",\n          \"description\": \"The relative resource name of the VMware Engine network.\"\n        }\n      }\n    },\n    \"managementCluster\": {\n      \"type\": \"object\",\n      \"description\": \"The management cluster for this private cloud.\",\n      \"properties\": {\n        \"clusterId\": {\n          \"type\": \"string\",\n          \"description\": \"The user-provided identifier of the management cluster.\"\n        },\n        \"nodeTypeConfigs\": {\n          \"type\": \"object\",\n          \"description\": \"Node type configurations for the management\
  \ cluster.\",\n          \"additionalProperties\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"nodeCount\": {\n                \"type\": \"integer\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Creation time of the resource.\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last update time of the resource.\"\n    },\n    \"expireTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time when the resource will be irreversibly purged.\"\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-vmware-engine/refs/heads/main/json-schema/vmwareengine-privatecloud.json
tags:
- Compute
- Google Cloud
- Migration
- Private Cloud
- Virtualization
- VMware
title: Google Cloud VMware Engine Private Cloud
---
