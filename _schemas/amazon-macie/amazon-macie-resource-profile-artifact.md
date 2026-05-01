---
description: Provides information about an S3 object that Amazon Macie selected for analysis while performing automated sensitive data discovery for an S3 bucket, and the status and results of the analysis. This information is available only if automated sensitive data discovery is currently enabled for your account.
layout: schema
name: ResourceProfileArtifact
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: classificationResultStatus
  type: object
- description: ''
  name: sensitive
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-resource-profile-artifact-schema.json
slug: amazon-macie-resource-profile-artifact
source_filename: amazon-macie-resource-profile-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-resource-profile-artifact-schema.json\",\n  \"title\": \"ResourceProfileArtifact\",\n  \"description\": \"Provides information about an S3 object that Amazon Macie selected for analysis while performing automated sensitive data discovery for an S3 bucket, and the status and results of the analysis. This information is available only if automated sensitive data discovery is currently enabled for your account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the object.\"\n        }\n      ]\n    },\n    \"classificationResultStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"description\": \"<p>The status of the analysis. Possible values are:</p> <ul><li><p>COMPLETE - Amazon Macie successfully completed its analysis of the object.</p></li> <li><p>PARTIAL - Macie analyzed only a subset of data in the object. For example, the object is an archive file that contains files in an unsupported format.</p></li> <li><p>SKIPPED - Macie wasn't able to analyze the object. For example, the object is a malformed file.</p></li></ul>\"\n        }\n      ]\n    },\n    \"sensitive\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether Amazon Macie found sensitive data in the object.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"classificationResultStatus\",\n    \"arn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-resource-profile-artifact-schema.json
tags:
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: ResourceProfileArtifact
---
