---
description: A Memorystore for Redis instance resource representing a fully managed Redis deployment on Google Cloud.
layout: schema
name: Google Cloud Memorystore for Redis Instance
properties_list:
- description: Unique name of the resource in the format projects/{project}/locations/{location}/instances/{instance}.
  name: name
  type: string
- description: An arbitrary user-provided name for the instance.
  name: displayName
  type: string
- description: Resource labels.
  name: labels
  type: object
- description: The zone where the instance will be provisioned.
  name: locationId
  type: string
- description: The alternative zone for a STANDARD_HA tier instance.
  name: alternativeLocationId
  type: string
- description: The version of Redis software.
  name: redisVersion
  type: string
- description: CIDR range of internal addresses reserved for this instance.
  name: reservedIpRange
  type: string
- description: Hostname or IP address of the exposed Redis endpoint.
  name: host
  type: string
- description: The port number of the exposed Redis endpoint.
  name: port
  type: integer
- description: The current state of the instance.
  name: state
  type: string
- description: Redis memory size in GiB.
  name: memorySizeGb
  type: integer
- description: The full name of the Google Compute Engine network to which the instance is connected.
  name: authorizedNetwork
  type: string
- description: The network connect mode of the Redis instance.
  name: connectMode
  type: string
- description: Whether AUTH is enabled for the instance.
  name: authEnabled
  type: boolean
- description: The service tier of the instance.
  name: tier
  type: string
- description: The number of replica nodes.
  name: replicaCount
  type: integer
- description: The TLS mode of the Redis instance.
  name: transitEncryptionMode
  type: string
- description: The creation time of the instance.
  name: createTime
  type: string
- description: Redis configuration parameters.
  name: redisConfigs
  type: object
provider_name: Google Cloud Memorystore
provider_slug: google-cloud-memorystore
schema_file: json-schema/instance-schema.json
slug: instance
source_filename: instance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-memorystore/refs/heads/main/json-schema/instance-schema.json\",\n  \"title\": \"Google Cloud Memorystore for Redis Instance\",\n  \"description\": \"A Memorystore for Redis instance resource representing a fully managed Redis deployment on Google Cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name of the resource in the format projects/{project}/locations/{location}/instances/{instance}.\",\n      \"pattern\": \"^projects/[^/]+/locations/[^/]+/instances/[^/]+$\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"An arbitrary user-provided name for the instance.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Resource labels.\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"The zone where the instance will be provisioned.\"\n    },\n    \"alternativeLocationId\": {\n      \"type\": \"string\",\n      \"description\": \"The alternative zone for a STANDARD_HA tier instance.\"\n    },\n    \"redisVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of Redis software.\",\n      \"examples\": [\"REDIS_6_X\", \"REDIS_7_0\"]\n    },\n    \"reservedIpRange\": {\n      \"type\": \"string\",\n      \"description\": \"CIDR range of internal addresses reserved for this instance.\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or IP address of the exposed Redis endpoint.\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"The port number of the exposed Redis endpoint.\",\n      \"default\": 6379\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\"\
  : [\"STATE_UNSPECIFIED\", \"CREATING\", \"READY\", \"UPDATING\", \"DELETING\", \"REPAIRING\", \"MAINTENANCE\", \"IMPORTING\", \"FAILING_OVER\"],\n      \"description\": \"The current state of the instance.\"\n    },\n    \"memorySizeGb\": {\n      \"type\": \"integer\",\n      \"description\": \"Redis memory size in GiB.\",\n      \"minimum\": 1\n    },\n    \"authorizedNetwork\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the Google Compute Engine network to which the instance is connected.\"\n    },\n    \"connectMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"CONNECT_MODE_UNSPECIFIED\", \"DIRECT_PEERING\", \"PRIVATE_SERVICE_ACCESS\"],\n      \"description\": \"The network connect mode of the Redis instance.\"\n    },\n    \"authEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether AUTH is enabled for the instance.\"\n    },\n    \"tier\": {\n      \"type\": \"string\",\n      \"enum\": [\"TIER_UNSPECIFIED\", \"BASIC\"\
  , \"STANDARD_HA\"],\n      \"description\": \"The service tier of the instance.\"\n    },\n    \"replicaCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of replica nodes.\",\n      \"minimum\": 0,\n      \"maximum\": 5\n    },\n    \"transitEncryptionMode\": {\n      \"type\": \"string\",\n      \"enum\": [\"TRANSIT_ENCRYPTION_MODE_UNSPECIFIED\", \"SERVER_AUTHENTICATION\", \"DISABLED\"],\n      \"description\": \"The TLS mode of the Redis instance.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The creation time of the instance.\"\n    },\n    \"redisConfigs\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Redis configuration parameters.\"\n    }\n  },\n  \"required\": [\"memorySizeGb\", \"tier\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-memorystore/refs/heads/main/json-schema/instance-schema.json
tags:
- Cache
- Google Cloud
- In-Memory
- Memcached
- Redis
title: Google Cloud Memorystore for Redis Instance
---
