---
description: DescribeJobResult schema from Amazon Snow Family API
layout: schema
name: DescribeJobResult
properties_list:
- description: ''
  name: JobMetadata
  type: object
- description: ''
  name: SubJobMetadata
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-describe-job-result-schema.json
slug: amazon-snow-family-describe-job-result
source_filename: amazon-snow-family-describe-job-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-job-result-schema.json\",\n  \"title\": \"DescribeJobResult\",\n  \"description\": \"DescribeJobResult schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobMetadata\"\n        },\n        {\n          \"description\": \"Information about a specific job, including shipping information, job status, and other important metadata.\"\n        }\n      ]\n    },\n    \"SubJobMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobMetadataList\"\n        },\n        {\n          \"description\": \"Information about a specific job part (in the case of an export job), including shipping information, job status, and\
  \ other important metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-describe-job-result-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: DescribeJobResult
---
