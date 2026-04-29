---
description: DescribeClustersResponse schema from Amazon MemoryDB API
layout: schema
name: DescribeClustersResponse
properties_list:
- description: A list of clusters.
  name: Clusters
  type: array
- description: An optional argument to pass in case the total number of records exceeds the value of MaxResults.
  name: NextToken
  type: string
provider_name: Amazon MemoryDB
provider_slug: amazon-memorydb
schema_file: json-schema/memorydb-api-describe-clusters-response-schema.json
slug: memorydb-api-describe-clusters-response
source_filename: memorydb-api-describe-clusters-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-describe-clusters-response-schema.json\",\n  \"title\": \"DescribeClustersResponse\",\n  \"description\": \"DescribeClustersResponse schema from Amazon MemoryDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Clusters\": {\n      \"description\": \"A list of clusters.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Cluster\"\n      },\n      \"type\": \"array\"\n    },\n    \"NextToken\": {\n      \"description\": \"An optional argument to pass in case the total number of records exceeds the value of MaxResults.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-memorydb/refs/heads/main/json-schema/memorydb-api-describe-clusters-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeClustersResponse
---
