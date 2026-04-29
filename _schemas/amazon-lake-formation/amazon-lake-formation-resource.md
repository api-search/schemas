---
description: A resource registered with AWS Lake Formation.
layout: schema
name: DataLakeResource
properties_list:
- description: The ARN of the resource registered with Lake Formation.
  name: ResourceArn
  type: string
- description: The IAM role that registered the resource.
  name: RoleArn
  type: string
- description: The date and time the resource was last modified.
  name: LastModified
  type: string
provider_name: Amazon Lake Formation
provider_slug: amazon-lake-formation
schema_file: json-schema/amazon-lake-formation-resource-schema.json
slug: amazon-lake-formation-resource
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lake-formation/refs/heads/main/json-schema/amazon-lake-formation-resource-schema.json\",\n  \"title\": \"DataLakeResource\",\n  \"description\": \"A resource registered with AWS Lake Formation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the resource registered with Lake Formation.\"\n    },\n    \"RoleArn\": {\n      \"type\": \"string\",\n      \"description\": \"The IAM role that registered the resource.\"\n    },\n    \"LastModified\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the resource was last modified.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lake-formation/refs/heads/main/json-schema/amazon-lake-formation-resource-schema.json
tags:
- Access Control
- Analytics
- AWS
- Data Governance
- Data Lake
- S3
title: DataLakeResource
---
