---
description: DescribeCodeCoveragesOutput schema from Amazon CodeBuild
layout: schema
name: DescribeCodeCoveragesOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: codeCoverages
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-describe-code-coverages-output-schema.json
slug: amazon-codebuild-describe-code-coverages-output
source_filename: amazon-codebuild-describe-code-coverages-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-describe-code-coverages-output-schema.json\",\n  \"title\": \"DescribeCodeCoveragesOutput\",\n  \"description\": \"DescribeCodeCoveragesOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"If there are more items to return, this contains a token that is passed to a subsequent call to <code>DescribeCodeCoverages</code> to retrieve the next set of items.\"\n        }\n      ]\n    },\n    \"codeCoverages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeCoverages\"\n        },\n        {\n          \"description\": \"An array of <code>CodeCoverage</code> objects that\
  \ contain the results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-describe-code-coverages-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DescribeCodeCoveragesOutput
---
