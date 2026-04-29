---
description: Specifies S3 buckets to add or remove from the exclusion list defined by the classification scope for an Amazon Macie account.
layout: schema
name: S3ClassificationScopeExclusionUpdate
properties_list:
- description: ''
  name: bucketNames
  type: object
- description: ''
  name: operation
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-s3-classification-scope-exclusion-update-schema.json
slug: amazon-macie-s3-classification-scope-exclusion-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-exclusion-update-schema.json\",\n  \"title\": \"S3ClassificationScopeExclusionUpdate\",\n  \"description\": \"Specifies S3 buckets to add or remove from the exclusion list defined by the classification scope for an Amazon Macie account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucketNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfS3BucketName\"\n        },\n        {\n          \"description\": \"Depending on the value specified for the update operation (ClassificationScopeUpdateOperation), an array of strings that: lists the names of buckets to add or remove from the list, or specifies a new set of bucket names that overwrites all existing names in the list. Each string must be the full name of an S3 bucket.\
  \ Values are case sensitive.\"\n        }\n      ]\n    },\n    \"operation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationScopeUpdateOperation\"\n        },\n        {\n          \"description\": \"<p>Specifies how to apply the changes to the exclusion list. Valid values are:</p> <ul><li><p>ADD - Append the specified bucket names to the current list.</p></li> <li><p>REMOVE - Remove the specified bucket names from the current list.</p></li> <li><p>REPLACE - Overwrite the current list with the specified list of bucket names. If you specify this value, Amazon Macie removes all existing names from the list and adds all the specified names to the list.</p></li></ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"bucketNames\",\n    \"operation\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-s3-classification-scope-exclusion-update-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: S3ClassificationScopeExclusionUpdate
---
