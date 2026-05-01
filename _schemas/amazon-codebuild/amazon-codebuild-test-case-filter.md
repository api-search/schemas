---
description: A filter used to return specific types of test cases. In order to pass the filter, the report must meet all of the filter properties.
layout: schema
name: TestCaseFilter
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: keyword
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-test-case-filter-schema.json
slug: amazon-codebuild-test-case-filter
source_filename: amazon-codebuild-test-case-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-test-case-filter-schema.json\",\n  \"title\": \"TestCaseFilter\",\n  \"description\": \"A filter used to return specific types of test cases. In order to pass the filter, the report must meet all of the filter properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>The status used to filter test cases. A <code>TestCaseFilter</code> can have one status. Valid values are:</p> <ul> <li> <p> <code>SUCCEEDED</code> </p> </li> <li> <p> <code>FAILED</code> </p> </li> <li> <p> <code>ERROR</code> </p> </li> <li> <p> <code>SKIPPED</code> </p> </li> <li> <p> <code>UNKNOWN</code> </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"keyword\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A keyword that is used to filter on the <code>name</code> or the <code>prefix</code> of the test cases. Only test cases where the keyword is a substring of the <code>name</code> or the <code>prefix</code> will be returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-test-case-filter-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: TestCaseFilter
---
