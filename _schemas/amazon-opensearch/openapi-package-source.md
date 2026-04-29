---
description: The S3 location for importing the package specified as <code>S3BucketName</code> and <code>S3Key</code>
layout: schema
name: PackageSource
properties_list:
- description: ''
  name: S3BucketName
  type: object
- description: ''
  name: S3Key
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-package-source-schema.json
slug: openapi-package-source
source_filename: openapi-package-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-package-source-schema.json\",\n  \"title\": \"PackageSource\",\n  \"description\": \"The S3 location for importing the package specified as <code>S3BucketName</code> and <code>S3Key</code>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"S3BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"Name of the bucket containing the package.\"\n        }\n      ]\n    },\n    \"S3Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Key\"\n        },\n        {\n          \"description\": \"Key (file name) of the package.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-package-source-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: PackageSource
---
