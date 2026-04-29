---
description: Metadata that is associated with a code review. This applies to both pull request and repository analysis code reviews.
layout: schema
name: RequestMetadata
properties_list:
- description: ''
  name: RequestId
  type: object
- description: ''
  name: Requester
  type: object
- description: ''
  name: EventInfo
  type: object
- description: ''
  name: VendorName
  type: object
provider_name: Amazon CodeGuru Reviewer
provider_slug: amazon-codeguru-reviewer
schema_file: json-schema/amazon-codeguru-reviewer-request-metadata-schema.json
slug: amazon-codeguru-reviewer-request-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-request-metadata-schema.json\",\n  \"title\": \"RequestMetadata\",\n  \"description\": \"Metadata that is associated with a code review. This applies to both pull request and repository analysis code reviews.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RequestId\"\n        },\n        {\n          \"description\": \"The ID of the request. This is required for a pull request code review.\"\n        }\n      ]\n    },\n    \"Requester\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Requester\"\n        },\n        {\n          \"description\": \"An identifier, such as a name or account ID, that is associated with the requester. The <code>Requester</code>\
  \ is used to capture the <code>author/actor</code> name of the event request.\"\n        }\n      ]\n    },\n    \"EventInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventInfo\"\n        },\n        {\n          \"description\": \"Information about the event associated with a code review.\"\n        }\n      ]\n    },\n    \"VendorName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VendorName\"\n        },\n        {\n          \"description\": \"The name of the repository vendor used to upload code to an S3 bucket for a CI/CD code review. For example, if code and artifacts are uploaded to an S3 bucket for a CI/CD code review by GitHub scripts from a GitHub repository, then the repository association's <code>ProviderType</code> is <code>S3Bucket</code> and the CI/CD repository vendor name is GitHub. For more information, see the definition for <code>ProviderType</code> in <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/reviewer-api/API_RepositoryAssociation.html\\\
  \">RepositoryAssociation</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-reviewer/refs/heads/main/json-schema/amazon-codeguru-reviewer-request-metadata-schema.json
tags:
- Amazon
- AWS
- Code Review
- Security
- DevOps
- Machine Learning
- Developer Tools
title: RequestMetadata
---
