---
description: CreateClusterResponse schema from Amazon MSK API
layout: schema
name: CreateClusterResponse
properties_list:
- description: ''
  name: ClusterArn
  type: object
- description: ''
  name: ClusterName
  type: object
- description: ''
  name: State
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-create-cluster-response-schema.json
slug: msk-api-create-cluster-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-create-cluster-response-schema.json\",\n  \"title\": \"CreateClusterResponse\",\n  \"description\": \"CreateClusterResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterArn\"\n          },\n          \"description\": \"\\n            <p>The Amazon Resource Name (ARN) of the cluster.</p>\"\n        }\n      ]\n    },\n    \"ClusterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterName\"\n          },\n          \"description\": \"\\n            <p>The name of the MSK\
  \ cluster.</p>\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"state\"\n          },\n          \"description\": \"\\n            <p>The state of the cluster. The possible states are ACTIVE, CREATING, DELETING, FAILED, HEALING, MAINTENANCE, REBOOTING_BROKER, and UPDATING.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-create-cluster-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateClusterResponse
---
