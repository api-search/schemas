---
description: An Elastigroup is a compute group that manages and optimizes cloud instances across spot, reserved, and on-demand capacity to ensure availability at the lowest cost.
layout: schema
name: Spot Elastigroup
properties_list:
- description: The unique identifier of the Elastigroup.
  name: id
  type: string
- description: The name of the Elastigroup.
  name: name
  type: string
- description: A description of the Elastigroup.
  name: description
  type: string
- description: The cloud provider region where the Elastigroup is deployed.
  name: region
  type: string
- description: The capacity configuration for the Elastigroup.
  name: capacity
  type: object
- description: The optimization strategy for the Elastigroup.
  name: strategy
  type: object
- description: The compute configuration for the Elastigroup.
  name: compute
  type: object
- description: The timestamp when the Elastigroup was created.
  name: createdAt
  type: string
- description: The timestamp when the Elastigroup was last updated.
  name: updatedAt
  type: string
provider_name: Spot
provider_slug: spot
schema_file: json-schema/elastigroup.json
slug: elastigroup
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/spot/blob/main/json-schema/elastigroup.json\",\n  \"title\": \"Spot Elastigroup\",\n  \"description\": \"An Elastigroup is a compute group that manages and optimizes cloud instances across spot, reserved, and on-demand capacity to ensure availability at the lowest cost.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the Elastigroup.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Elastigroup.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the Elastigroup.\"\n    },\n    \"region\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider region where the Elastigroup is deployed.\"\n    },\n    \"capacity\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"The capacity configuration for the Elastigroup.\",\n      \"properties\": {\n        \"target\": {\n          \"type\": \"integer\",\n          \"description\": \"The desired number of instances.\"\n        },\n        \"minimum\": {\n          \"type\": \"integer\",\n          \"description\": \"The minimum number of instances.\"\n        },\n        \"maximum\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of instances.\"\n        },\n        \"unit\": {\n          \"type\": \"string\",\n          \"enum\": [\"instance\", \"weight\"],\n          \"description\": \"The unit of capacity measurement.\"\n        }\n      }\n    },\n    \"strategy\": {\n      \"type\": \"object\",\n      \"description\": \"The optimization strategy for the Elastigroup.\",\n      \"properties\": {\n        \"risk\": {\n          \"type\": \"integer\",\n          \"description\": \"Percentage of spot instances (0-100).\"\n        },\n       \
  \ \"onDemandCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of on-demand instances to maintain.\"\n        },\n        \"availabilityVsCost\": {\n          \"type\": \"string\",\n          \"enum\": [\"balanced\", \"costOriented\", \"availabilityOriented\", \"cheapest\"],\n          \"description\": \"The optimization preference between availability and cost.\"\n        },\n        \"fallbackToOd\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to fall back to on-demand instances when spot is unavailable.\"\n        },\n        \"utilizeReservedInstances\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to utilize reserved instances when available.\"\n        }\n      }\n    },\n    \"compute\": {\n      \"type\": \"object\",\n      \"description\": \"The compute configuration for the Elastigroup.\",\n      \"properties\": {\n        \"instanceTypes\": {\n          \"type\": \"object\",\n         \
  \ \"properties\": {\n            \"ondemand\": {\n              \"type\": \"string\",\n              \"description\": \"The on-demand instance type.\"\n            },\n            \"spot\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              },\n              \"description\": \"The spot instance types to consider.\"\n            }\n          }\n        },\n        \"availabilityZones\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\"\n              },\n              \"subnetId\": {\n                \"type\": \"string\"\n              }\n            }\n          },\n          \"description\": \"The availability zones for the Elastigroup.\"\n        }\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp\
  \ when the Elastigroup was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the Elastigroup was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/spot/refs/heads/main/json-schema/elastigroup.json
tags:
- Autoscaling
- Cloud Infrastructure
- Containers
- Cost Optimization
- FinOps
- Kubernetes
- Spot Instances
title: Spot Elastigroup
---
