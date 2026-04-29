---
description: Information about the application.
layout: schema
name: Application
properties_list:
- description: The application Amazon Resource Name (ARN).
  name: applicationId
  type: string
- description: The name of the application.
  name: name
  type: string
- description: The name of the author publishing the app.
  name: author
  type: string
- description: The description of the application.
  name: description
  type: string
- description: The date and time this resource was created.
  name: creationTime
  type: string
- description: A URL with more information about the application.
  name: homePageUrl
  type: string
- description: Labels to improve discovery of apps in search results.
  name: labels
  type: array
- description: A link to a license file of the app.
  name: licenseUrl
  type: string
- description: A link to the readme file in Markdown language.
  name: readmeUrl
  type: string
- description: A valid identifier from https://spdx.org/licenses/.
  name: spdxLicenseId
  type: string
- description: ''
  name: version
  type: object
provider_name: Amazon Serverless Application Repository
provider_slug: amazon-serverless-application-repository
schema_file: json-schema/amazon-serverless-application-repository-application-schema.json
slug: amazon-serverless-application-repository-application
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-application-schema.json\",\n  \"title\": \"Application\",\n  \"description\": \"Information about the application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"The application Amazon Resource Name (ARN).\",\n      \"example\": \"arn:aws:serverlessrepo:us-east-1:123456789012:applications/MyApp\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application.\",\n      \"example\": \"MyApp\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the author publishing the app.\",\n      \"example\": \"developer@example.com\"\n    },\n    \"description\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The description of the application.\",\n      \"example\": \"A sample serverless application\"\n    },\n    \"creationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time this resource was created.\"\n    },\n    \"homePageUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A URL with more information about the application.\"\n    },\n    \"labels\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Labels to improve discovery of apps in search results.\"\n    },\n    \"licenseUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A link to a license file of the app.\"\n    },\n    \"readmeUrl\": {\n      \"type\": \"string\",\n      \"description\": \"A link to the readme file in Markdown language.\"\n    },\n    \"spdxLicenseId\": {\n      \"type\": \"string\",\n      \"description\": \"A valid identifier\
  \ from https://spdx.org/licenses/.\"\n    },\n    \"version\": {\n      \"$ref\": \"#/components/schemas/VersionSummary\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-serverless-application-repository/refs/heads/main/json-schema/amazon-serverless-application-repository-application-schema.json
tags:
- Application Repository
- AWS
- Lambda
- SAM
- Serverless
title: Application
---
