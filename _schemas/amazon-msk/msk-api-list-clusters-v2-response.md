---
description: ListClustersV2Response schema from Amazon MSK API
layout: schema
name: ListClustersV2Response
properties_list:
- description: ''
  name: ClusterInfoList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-list-clusters-v2-response-schema.json
slug: msk-api-list-clusters-v2-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-clusters-v2-response-schema.json\",\n  \"title\": \"ListClustersV2Response\",\n  \"description\": \"ListClustersV2Response schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfCluster\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterInfoList\"\n          },\n          \"description\": \"\\n            <p>Information on each of the MSK clusters in the response.</p>\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"\\n      \
  \      <p>The paginated results marker. When the result of a ListClusters operation is truncated, the call returns NextToken in the response. \\n               To get another batch of clusters, provide this token in your next request.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-list-clusters-v2-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListClustersV2Response
---
