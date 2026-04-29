---
description: DescribeCodeCoveragesInput schema from Amazon CodeBuild
layout: schema
name: DescribeCodeCoveragesInput
properties_list:
- description: ''
  name: reportArn
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: minLineCoveragePercentage
  type: object
- description: ''
  name: maxLineCoveragePercentage
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-describe-code-coverages-input-schema.json
slug: amazon-codebuild-describe-code-coverages-input
source_filename: amazon-codebuild-describe-code-coverages-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-describe-code-coverages-input-schema.json\",\n  \"title\": \"DescribeCodeCoveragesInput\",\n  \"description\": \"DescribeCodeCoveragesInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the report for which test cases are returned. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> value returned from a previous call to <code>DescribeCodeCoverages</code>. This specifies the next item to return. To return the beginning\
  \ of the list, exclude this parameter.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrderType\"\n        },\n        {\n          \"description\": \"Specifies if the results are sorted in ascending or descending order.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportCodeCoverageSortByType\"\n        },\n        {\n          \"description\": \"<p>Specifies how the results are sorted. Possible values are:</p> <dl> <dt>FILE_PATH</dt> <dd> <p>The results are sorted by file path.</p> </dd> <dt>LINE_COVERAGE_PERCENTAGE</dt> <dd> <p>The results are sorted by the percentage of lines that are covered.</p>\
  \ </dd> </dl>\"\n        }\n      ]\n    },\n    \"minLineCoveragePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The minimum line coverage percentage to report.\"\n        }\n      ]\n    },\n    \"maxLineCoveragePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The maximum line coverage percentage to report.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"reportArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-describe-code-coverages-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: DescribeCodeCoveragesInput
---
