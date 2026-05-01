---
description: Information about an associated repository in an S3 bucket. The associated repository contains a source code .zip file and a build artifacts .zip file that contains .jar or .class files.
layout: schema
name: S3BucketRepository
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Details
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-s3-bucket-repository-schema.json
slug: amazon-codeguru-reviewer-s3-bucket-repository
source_filename: amazon-codeguru-reviewer-s3-bucket-repository-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-s3-bucket-repository-schema.json\",\n  \"title\": \"S3BucketRepository\",\n  \"description\": \"Information about an associated repository in an S3 bucket. The associated repository contains a source code .zip file and a build artifacts .zip file that contains .jar or .class files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the repository when the <code>ProviderType</code> is <code>S3Bucket</code>.\"\n        }\n      ]\n    },\n    \"Details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3RepositoryDetails\"\n        },\n        {\n          \"description\": \"An <code>S3RepositoryDetails</code>\
  \ object that specifies the name of an S3 bucket and a <code>CodeArtifacts</code> object. The <code>CodeArtifacts</code> object includes the S3 object keys for a source code .zip file and for a build artifacts .zip file.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-s3-bucket-repository-schema.json
tags:
- Amazon
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: S3BucketRepository
---
