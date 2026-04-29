---
description: CreateClusterV2Request schema from Amazon MSK API
layout: schema
name: CreateClusterV2Request
properties_list:
- description: ''
  name: ClusterName
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: Provisioned
  type: object
- description: ''
  name: Serverless
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-create-cluster-v2-request-schema.json
slug: msk-api-create-cluster-v2-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-create-cluster-v2-request-schema.json\",\n  \"title\": \"CreateClusterV2Request\",\n  \"description\": \"CreateClusterV2Request schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1Max64\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterName\"\n          },\n          \"description\": \"\\n            <p>The name of the cluster.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__mapOf__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"\\n            <p>A map of tags that you want the cluster\
  \ to have.</p>\"\n        }\n      ]\n    },\n    \"Provisioned\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisionedRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"provisioned\"\n          },\n          \"description\": \"\\n            <p>Information about the provisioned cluster.</p>\"\n        }\n      ]\n    },\n    \"Serverless\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerlessRequest\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serverless\"\n          },\n          \"description\": \"\\n            <p>Information about the serverless cluster.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClusterName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-create-cluster-v2-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateClusterV2Request
---
