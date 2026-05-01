---
description: DescribeVolumesResult schema from Amazon EBS Amazon Elastic Block Store (EBS) API
layout: schema
name: DescribeVolumesResult
properties_list:
- description: ''
  name: volumeSet
  type: array
- description: ''
  name: nextToken
  type: string
provider_name: Amazon EBS
provider_slug: amazon-ebs
schema_file: json-schema/ebs-openapi-describe-volumes-result-schema.json
slug: ebs-openapi-describe-volumes-result
source_filename: ebs-openapi-describe-volumes-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/json-schema/ebs-openapi-describe-volumes-result-schema.json\",\n  \"title\": \"DescribeVolumesResult\",\n  \"description\": \"DescribeVolumesResult schema from Amazon EBS Amazon Elastic Block Store (EBS) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"volumeSet\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Volume\"\n      }\n    },\n    \"nextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ebs/refs/heads/main/json-schema/ebs-openapi-describe-volumes-result-schema.json
tags:
- Amazon Web Services
- Block Storage
- EBS
- EC2
- Snapshots
- Storage
- Volumes
title: DescribeVolumesResult
---
