---
description: <p>Contains code coverage report information.</p> <p>Line coverage measures how many statements your tests cover. A statement is a single instruction, not including comments, conditionals, etc.</p> <p>Branch coverage determines if your tests cover every possible branch of a control structure, such as an <code>if</code> or <code>case</code> statement.</p>
layout: schema
name: CodeCoverage
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: reportARN
  type: object
- description: ''
  name: filePath
  type: object
- description: ''
  name: lineCoveragePercentage
  type: object
- description: ''
  name: linesCovered
  type: object
- description: ''
  name: linesMissed
  type: object
- description: ''
  name: branchCoveragePercentage
  type: object
- description: ''
  name: branchesCovered
  type: object
- description: ''
  name: branchesMissed
  type: object
- description: ''
  name: expired
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-code-coverage-schema.json
slug: amazon-codebuild-code-coverage
source_filename: amazon-codebuild-code-coverage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-code-coverage-schema.json\",\n  \"title\": \"CodeCoverage\",\n  \"description\": \"<p>Contains code coverage report information.</p> <p>Line coverage measures how many statements your tests cover. A statement is a single instruction, not including comments, conditionals, etc.</p> <p>Branch coverage determines if your tests cover every possible branch of a control structure, such as an <code>if</code> or <code>case</code> statement.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The identifier of the code coverage report.\"\n        }\n      ]\n    },\n    \"reportARN\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the report.\"\n        }\n      ]\n    },\n    \"filePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The path of the test report file.\"\n        }\n      ]\n    },\n    \"lineCoveragePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of lines that are covered by your tests.\"\n        }\n      ]\n    },\n    \"linesCovered\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of lines that are covered by your tests.\"\n        }\n      ]\n    },\n    \"linesMissed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\
  \n        },\n        {\n          \"description\": \"The number of lines that are not covered by your tests.\"\n        }\n      ]\n    },\n    \"branchCoveragePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of branches that are covered by your tests.\"\n        }\n      ]\n    },\n    \"branchesCovered\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of conditional branches that are covered by your tests.\"\n        }\n      ]\n    },\n    \"branchesMissed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of conditional branches that are not covered by your tests.\"\n        }\n      ]\n    },\n    \"expired\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time that the tests were run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-code-coverage-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CodeCoverage
---
