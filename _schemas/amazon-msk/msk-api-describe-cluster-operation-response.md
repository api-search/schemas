---
description: DescribeClusterOperationResponse schema from Amazon MSK API
layout: schema
name: DescribeClusterOperationResponse
properties_list:
- description: ''
  name: ClusterOperationInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-describe-cluster-operation-response-schema.json
slug: msk-api-describe-cluster-operation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-describe-cluster-operation-response-schema.json\",\n  \"title\": \"DescribeClusterOperationResponse\",\n  \"description\": \"DescribeClusterOperationResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterOperationInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterOperationInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterOperationInfo\"\n          },\n          \"description\": \"\\n            <p>Cluster operation information</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-describe-cluster-operation-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeClusterOperationResponse
---
