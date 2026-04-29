---
description: DescribeClusterResponse schema from Amazon MSK API
layout: schema
name: DescribeClusterResponse
properties_list:
- description: ''
  name: ClusterInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-describe-cluster-response-schema.json
slug: msk-api-describe-cluster-response
source_filename: msk-api-describe-cluster-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-describe-cluster-response-schema.json\",\n  \"title\": \"DescribeClusterResponse\",\n  \"description\": \"DescribeClusterResponse schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterInfo\"\n          },\n          \"description\": \"\\n            <p>The cluster information.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-describe-cluster-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeClusterResponse
---
