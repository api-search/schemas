---
description: ''
layout: schema
name: ListJobsResult
properties_list:
- description: ''
  name: Jobs
  type: array
- description: ''
  name: NextToken
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-list-jobs-result-schema.json
slug: amazon-s3-control-list-jobs-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListJobsResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"type\": \"array\"\n    },\n    \"NextToken\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-list-jobs-result-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: ListJobsResult
---
