---
description: Information about a test case created using a framework such as NUnit or Cucumber. A test case might be a unit test or a configuration test.
layout: schema
name: TestCase
properties_list:
- description: ''
  name: reportArn
  type: object
- description: ''
  name: testRawDataPath
  type: object
- description: ''
  name: prefix
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: durationInNanoSeconds
  type: object
- description: ''
  name: message
  type: object
- description: ''
  name: expired
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-test-case-schema.json
slug: amazon-codebuild-test-case
source_filename: amazon-codebuild-test-case-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-test-case-schema.json\",\n  \"title\": \"TestCase\",\n  \"description\": \" Information about a test case created using a framework such as NUnit or Cucumber. A test case might be a unit test or a configuration test. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"reportArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The ARN of the report to which the test case belongs. \"\n        }\n      ]\n    },\n    \"testRawDataPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The path to the raw data file that contains the test result. \"\n        }\n      ]\n    },\n    \"prefix\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A string that is applied to a series of related test cases. CodeBuild generates the prefix. The prefix depends on the framework used to generate the tests. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The name of the test case. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The status returned by the test case after it was run. Valid statuses are <code>SUCCEEDED</code>, <code>FAILED</code>, <code>ERROR</code>, <code>SKIPPED</code>, and <code>UNKNOWN</code>. \"\n        }\n      ]\n    },\n    \"durationInNanoSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/WrapperLong\"\n        },\n        {\n          \"description\": \" The number of nanoseconds it took to run this test case. \"\n        }\n      ]\n    },\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" A message associated with a test case. For example, an error message or stack trace. \"\n        }\n      ]\n    },\n    \"expired\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" The date and time a test case expires. A test case expires 30 days after it is created. An expired test case is not available to view in CodeBuild. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-test-case-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: TestCase
---
