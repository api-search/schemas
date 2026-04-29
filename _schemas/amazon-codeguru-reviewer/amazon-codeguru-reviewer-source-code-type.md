---
description: Specifies the source code that is analyzed in a code review.
layout: schema
name: SourceCodeType
properties_list:
- description: ''
  name: CommitDiff
  type: object
- description: ''
  name: RepositoryHead
  type: object
- description: ''
  name: BranchDiff
  type: object
- description: ''
  name: S3BucketRepository
  type: object
- description: ''
  name: RequestMetadata
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-source-code-type-schema.json
slug: amazon-codeguru-reviewer-source-code-type
source_filename: amazon-codeguru-reviewer-source-code-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-source-code-type-schema.json\",\n  \"title\": \"SourceCodeType\",\n  \"description\": \"Specifies the source code that is analyzed in a code review.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CommitDiff\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommitDiffSourceCodeType\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> that specifies a commit diff created by a pull request on an associated repository.\"\n        }\n      ]\n    },\n    \"RepositoryHead\": {\n      \"$ref\": \"#/components/schemas/RepositoryHeadSourceCodeType\"\n    },\n    \"BranchDiff\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/BranchDiffSourceCodeType\"\n        },\n        {\n          \"description\": \"A type of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> that specifies a source branch name and a destination branch name in an associated repository.\"\n        }\n      ]\n    },\n    \"S3BucketRepository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketRepository\"\n        },\n        {\n          \"description\": \"Information about an associated repository in an S3 bucket that includes its name and an <code>S3RepositoryDetails</code> object. The <code>S3RepositoryDetails</code> object includes the name of an S3 bucket, an S3 key for a source code .zip file, and an S3 key for a build artifacts .zip file. <code>S3BucketRepository</code> is required in <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_SourceCodeType\\\">SourceCodeType</a> for <code>S3BucketRepository</code>\
  \ based code reviews.\"\n        }\n      ]\n    },\n    \"RequestMetadata\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestMetadata\"\n        },\n        {\n          \"description\": \"Metadata that is associated with a code review. This applies to any type of code review supported by CodeGuru Reviewer. The <code>RequestMetadaa</code> field captures any event metadata. For example, it might capture metadata associated with an event trigger, such as a push or a pull request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-source-code-type-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: SourceCodeType
---
