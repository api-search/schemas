---
description: Information about a repository in an S3 bucket.
layout: schema
name: S3Repository
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: BucketName
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-s3-repository-schema.json
slug: amazon-codeguru-reviewer-s3-repository
source_filename: amazon-codeguru-reviewer-s3-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-s3-repository-schema.json\",\n  \"title\": \"S3Repository\",\n  \"description\": \"Information about a repository in an S3 bucket.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the repository in the S3 bucket.\"\n        }\n      ]\n    },\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The name of the S3 bucket used for associating a new S3 repository. It must begin with <code>codeguru-reviewer-</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"BucketName\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-s3-repository-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: S3Repository
---
