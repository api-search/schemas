---
description: DescribeClusterResult schema from Amazon Snow Family API
layout: schema
name: DescribeClusterResult
properties_list:
- description: ''
  name: ClusterMetadata
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-cluster-result-schema.json
slug: amazon-snow-family-describe-cluster-result
source_filename: amazon-snow-family-describe-cluster-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-cluster-result-schema.json\",\n  \"title\": \"DescribeClusterResult\",\n  \"description\": \"DescribeClusterResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterMetadata\"\n        },\n        {\n          \"description\": \"Information about a specific cluster, including shipping information, cluster status, and other important metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-cluster-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeClusterResult
---
