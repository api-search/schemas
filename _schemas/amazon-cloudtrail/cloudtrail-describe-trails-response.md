---
description: DescribeTrailsResponse schema
layout: schema
name: DescribeTrailsResponse
properties_list:
- description: ''
  name: trailList
  type: array
provider_name: Amazon CloudTrail
provider_slug: amazon-cloudtrail
schema_file: json-schema/cloudtrail-describe-trails-response-schema.json
slug: cloudtrail-describe-trails-response
source_filename: cloudtrail-describe-trails-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-describe-trails-response-schema.json\",\n  \"title\": \"DescribeTrailsResponse\",\n  \"description\": \"DescribeTrailsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"trailList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Name\": {\n            \"type\": \"string\"\n          },\n          \"S3BucketName\": {\n            \"type\": \"string\"\n          },\n          \"TrailARN\": {\n            \"type\": \"string\"\n          },\n          \"HomeRegion\": {\n            \"type\": \"string\"\n          },\n          \"IsMultiRegionTrail\": {\n            \"type\": \"boolean\"\n          },\n          \"LogFileValidationEnabled\": {\n            \"type\": \"boolean\"\n          },\n       \
  \   \"HasCustomEventSelectors\": {\n            \"type\": \"boolean\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudtrail/refs/heads/main/json-schema/cloudtrail-describe-trails-response-schema.json
tags:
- CloudTrail
- Audit
- Compliance
- Governance
- Security
title: DescribeTrailsResponse
---
