---
description: CreateCodeReviewRequest schema from Amazon CodeGuru Reviewer
layout: schema
name: CreateCodeReviewRequest
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: RepositoryAssociationArn
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: ClientRequestToken
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-create-code-review-request-schema.json
slug: amazon-codeguru-reviewer-create-code-review-request
source_filename: amazon-codeguru-reviewer-create-code-review-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-create-code-review-request-schema.json\",\n  \"title\": \"CreateCodeReviewRequest\",\n  \"description\": \"CreateCodeReviewRequest schema from Amazon CodeGuru Reviewer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeReviewName\"\n        },\n        {\n          \"description\": \"The name of the code review. The name of each code review in your Amazon Web Services account must be unique.\"\n        }\n      ]\n    },\n    \"RepositoryAssociationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssociationArn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociation.html\\\
  \">RepositoryAssociation</a> object. You can retrieve this ARN by calling <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_ListRepositoryAssociations.html\\\">ListRepositoryAssociations</a>.</p> <p>A code review can only be created on an associated repository. This is the ARN of the associated repository.</p>\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeReviewType\"\n        },\n        {\n          \"description\": \"The type of code review to create. This is specified using a <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_CodeReviewType.html\\\">CodeReviewType</a> object. You can create a code review only of type <code>RepositoryAnalysis</code>.\"\n        }\n      ]\n    },\n    \"ClientRequestToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientRequestToken\"\n        },\n        {\n          \"description\": \"Amazon\
  \ CodeGuru Reviewer uses this value to prevent the accidental creation of duplicate code reviews if there are failures and retries.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RepositoryAssociationArn\",\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-create-code-review-request-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: CreateCodeReviewRequest
---
