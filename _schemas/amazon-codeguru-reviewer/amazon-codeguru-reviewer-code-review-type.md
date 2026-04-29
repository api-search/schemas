---
description: <p>The type of a code review. There are two code review types:</p> <ul> <li> <p> <code>PullRequest</code> - A code review that is automatically triggered by a pull request on an associated repository.</p> </li> <li> <p> <code>RepositoryAnalysis</code> - A code review that analyzes all code under a specified branch in an associated repository. The associated repository is specified using its ARN in <a href="https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CreateCodeReview">CreateCodeReview</a>.</p> </li> </ul>
layout: schema
name: CodeReviewType
properties_list:
- description: ''
  name: RepositoryAnalysis
  type: object
- description: ''
  name: AnalysisTypes
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-code-review-type-schema.json
slug: amazon-codeguru-reviewer-code-review-type
source_filename: amazon-codeguru-reviewer-code-review-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-review-type-schema.json\",\n  \"title\": \"CodeReviewType\",\n  \"description\": \"<p>The type of a code review. There are two code review types:</p> <ul> <li> <p> <code>PullRequest</code> - A code review that is automatically triggered by a pull request on an associated repository.</p> </li> <li> <p> <code>RepositoryAnalysis</code> - A code review that analyzes all code under a specified branch in an associated repository. The associated repository is specified using its ARN in <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CreateCodeReview\\\">CreateCodeReview</a>.</p> </li> </ul>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RepositoryAnalysis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryAnalysis\"\
  \n        },\n        {\n          \"description\": \"A code review that analyzes all code under a specified branch in an associated repository. The associated repository is specified using its ARN in <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CreateCodeReview\\\">CreateCodeReview</a>.\"\n        }\n      ]\n    },\n    \"AnalysisTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AnalysisTypes\"\n        },\n        {\n          \"description\": \"They types of analysis performed during a repository analysis or a pull request review. You can specify either <code>Security</code>, <code>CodeQuality</code>, or both.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RepositoryAnalysis\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-code-review-type-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: CodeReviewType
---
