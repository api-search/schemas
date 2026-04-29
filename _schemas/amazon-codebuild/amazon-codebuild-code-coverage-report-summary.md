---
description: <p>Contains a summary of a code coverage report.</p> <p>Line coverage measures how many statements your tests cover. A statement is a single instruction, not including comments, conditionals, etc.</p> <p>Branch coverage determines if your tests cover every possible branch of a control structure, such as an <code>if</code> or <code>case</code> statement.</p>
layout: schema
name: CodeCoverageReportSummary
properties_list:
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
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-code-coverage-report-summary-schema.json
slug: amazon-codebuild-code-coverage-report-summary
source_filename: amazon-codebuild-code-coverage-report-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-code-coverage-report-summary-schema.json\",\n  \"title\": \"CodeCoverageReportSummary\",\n  \"description\": \"<p>Contains a summary of a code coverage report.</p> <p>Line coverage measures how many statements your tests cover. A statement is a single instruction, not including comments, conditionals, etc.</p> <p>Branch coverage determines if your tests cover every possible branch of a control structure, such as an <code>if</code> or <code>case</code> statement.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lineCoveragePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of lines that are covered by your tests.\"\n        }\n      ]\n    },\n    \"linesCovered\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of lines that are covered by your tests.\"\n        }\n      ]\n    },\n    \"linesMissed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of lines that are not covered by your tests.\"\n        }\n      ]\n    },\n    \"branchCoveragePercentage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Percentage\"\n        },\n        {\n          \"description\": \"The percentage of branches that are covered by your tests.\"\n        }\n      ]\n    },\n    \"branchesCovered\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of conditional branches that are covered by your tests.\"\n   \
  \     }\n      ]\n    },\n    \"branchesMissed\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonNegativeInt\"\n        },\n        {\n          \"description\": \"The number of conditional branches that are not covered by your tests.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-code-coverage-report-summary-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: CodeCoverageReportSummary
---
