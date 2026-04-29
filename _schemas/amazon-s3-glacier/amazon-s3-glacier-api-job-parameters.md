---
description: JobParameters schema from api
layout: schema
name: JobParameters
properties_list:
- description: ''
  name: Type
  type: string
- description: ''
  name: ArchiveId
  type: string
- description: ''
  name: Description
  type: string
- description: ''
  name: SNSTopic
  type: string
- description: ''
  name: RetrievalByteRange
  type: string
- description: ''
  name: Tier
  type: string
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
schema_file: json-schema/amazon-s3-glacier-api-job-parameters-schema.json
slug: amazon-s3-glacier-api-job-parameters
source_filename: amazon-s3-glacier-api-job-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-api-job-parameters-schema.json\",\n  \"title\": \"JobParameters\",\n  \"description\": \"JobParameters schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"archive-retrieval\",\n        \"inventory-retrieval\",\n        \"select\"\n      ]\n    },\n    \"ArchiveId\": {\n      \"type\": \"string\"\n    },\n    \"Description\": {\n      \"type\": \"string\"\n    },\n    \"SNSTopic\": {\n      \"type\": \"string\"\n    },\n    \"RetrievalByteRange\": {\n      \"type\": \"string\"\n    },\n    \"Tier\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Expedited\",\n        \"Standard\",\n        \"Bulk\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-api-job-parameters-schema.json
tags:
- Archive
- AWS
- Backup
- Storage
title: JobParameters
---
