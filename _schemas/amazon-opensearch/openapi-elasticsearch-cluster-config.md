---
description: Specifies the configuration for the domain cluster, such as the type and number of instances.
layout: schema
name: ElasticsearchClusterConfig
properties_list:
- description: ''
  name: InstanceType
  type: object
- description: ''
  name: InstanceCount
  type: object
- description: ''
  name: DedicatedMasterEnabled
  type: object
- description: ''
  name: ZoneAwarenessEnabled
  type: object
- description: ''
  name: ZoneAwarenessConfig
  type: object
- description: ''
  name: DedicatedMasterType
  type: object
- description: ''
  name: DedicatedMasterCount
  type: object
- description: ''
  name: WarmEnabled
  type: object
- description: ''
  name: WarmType
  type: object
- description: ''
  name: WarmCount
  type: object
- description: ''
  name: ColdStorageOptions
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-elasticsearch-cluster-config-schema.json
slug: openapi-elasticsearch-cluster-config
source_filename: openapi-elasticsearch-cluster-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-elasticsearch-cluster-config-schema.json\",\n  \"title\": \"ElasticsearchClusterConfig\",\n  \"description\": \"Specifies the configuration for the domain cluster, such as the type and number of instances.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ESPartitionInstanceType\"\n        },\n        {\n          \"description\": \"The instance type for an Elasticsearch cluster. UltraWarm instance types are not supported for data instances.\"\n        }\n      ]\n    },\n    \"InstanceCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"The number of instances in the specified domain cluster.\"\n\
  \        }\n      ]\n    },\n    \"DedicatedMasterEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A boolean value to indicate whether a dedicated master node is enabled. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-managedomains.html#es-managedomains-dedicatedmasternodes\\\" target=\\\"_blank\\\">About Dedicated Master Nodes</a> for more information.\"\n        }\n      ]\n    },\n    \"ZoneAwarenessEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"A boolean value to indicate whether zone awareness is enabled. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-managedomains.html#es-managedomains-zoneawareness\\\" target=\\\"_blank\\\">About Zone Awareness</a> for more information.\"\n        }\n      ]\n\
  \    },\n    \"ZoneAwarenessConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ZoneAwarenessConfig\"\n        },\n        {\n          \"description\": \"Specifies the zone awareness configuration for a domain when zone awareness is enabled.\"\n        }\n      ]\n    },\n    \"DedicatedMasterType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ESPartitionInstanceType\"\n        },\n        {\n          \"description\": \"The instance type for a dedicated master node.\"\n        }\n      ]\n    },\n    \"DedicatedMasterCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"Total number of dedicated master nodes, active and on standby, for the cluster.\"\n        }\n      ]\n    },\n    \"WarmEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n         \
  \ \"description\": \"True to enable warm storage.\"\n        }\n      ]\n    },\n    \"WarmType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ESWarmPartitionInstanceType\"\n        },\n        {\n          \"description\": \"The instance type for the Elasticsearch cluster's warm nodes.\"\n        }\n      ]\n    },\n    \"WarmCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntegerClass\"\n        },\n        {\n          \"description\": \"The number of warm nodes in the cluster.\"\n        }\n      ]\n    },\n    \"ColdStorageOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ColdStorageOptions\"\n        },\n        {\n          \"description\": \"Specifies the <code>ColdStorageOptions</code> config for Elasticsearch Domain\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-elasticsearch-cluster-config-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ElasticsearchClusterConfig
---
