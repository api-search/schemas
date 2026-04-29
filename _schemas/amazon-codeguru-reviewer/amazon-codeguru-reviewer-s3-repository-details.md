---
description: Specifies the name of an S3 bucket and a <code>CodeArtifacts</code> object that contains the S3 object keys for a source code .zip file and for a build artifacts .zip file that contains .jar or .class files.
layout: schema
name: S3RepositoryDetails
properties_list:
- description: ''
  name: BucketName
  type: object
- description: ''
  name: CodeArtifacts
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-s3-repository-details-schema.json
slug: amazon-codeguru-reviewer-s3-repository-details
source_filename: amazon-codeguru-reviewer-s3-repository-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-s3-repository-details-schema.json\",\n  \"title\": \"S3RepositoryDetails\",\n  \"description\": \"Specifies the name of an S3 bucket and a <code>CodeArtifacts</code> object that contains the S3 object keys for a source code .zip file and for a build artifacts .zip file that contains .jar or .class files.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BucketName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketName\"\n        },\n        {\n          \"description\": \"The name of the S3 bucket used for associating a new S3 repository. It must begin with <code>codeguru-reviewer-</code>. \"\n        }\n      ]\n    },\n    \"CodeArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeArtifacts\"\
  \n        },\n        {\n          \"description\": \"A <code>CodeArtifacts</code> object. The <code>CodeArtifacts</code> object includes the S3 object key for a source code .zip file and for a build artifacts .zip file that contains .jar or .class files.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-s3-repository-details-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: S3RepositoryDetails
---
