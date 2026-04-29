---
description: ListClusterOperationsResponse schema from Amazon MSK API
layout: schema
name: ListClusterOperationsResponse
properties_list:
- description: ''
  name: ClusterOperationInfoList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-cluster-operations-response-schema.json
slug: msk-api-list-cluster-operations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-cluster-operations-response-schema.json\",\n  \"title\": \"ListClusterOperationsResponse\",\n  \"description\": \"ListClusterOperationsResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterOperationInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfClusterOperationInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterOperationInfoList\"\n          },\n          \"description\": \"\\n            <p>An array of cluster operation information objects.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n      \
  \    },\n          \"description\": \"\\n            <p>If the response of ListClusterOperations is truncated, it returns a NextToken in the response. This Nexttoken should be sent in the subsequent request to ListClusterOperations.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-cluster-operations-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListClusterOperationsResponse
---
