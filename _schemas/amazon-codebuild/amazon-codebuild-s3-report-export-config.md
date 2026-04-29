---
description: Information about the S3 bucket where the raw data of a report are exported.
layout: schema
name: S3ReportExportConfig
properties_list:
- description: ''
  name: bucket
  type: object
- description: ''
  name: bucketOwner
  type: object
- description: ''
  name: path
  type: object
- description: ''
  name: packaging
  type: object
- description: ''
  name: encryptionKey
  type: object
- description: ''
  name: encryptionDisabled
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-s3-report-export-config-schema.json
slug: amazon-codebuild-s3-report-export-config
source_filename: amazon-codebuild-s3-report-export-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-s3-report-export-config-schema.json\",\n  \"title\": \"S3ReportExportConfig\",\n  \"description\": \" Information about the S3 bucket where the raw data of a report are exported. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \" The name of the S3 bucket where the raw data of a report are exported. \"\n        }\n      ]\n    },\n    \"bucketOwner\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account identifier of the owner of the Amazon S3 bucket. This allows report data to be exported to an Amazon S3 bucket\
  \ that is owned by an account other than the account running the build.\"\n        }\n      ]\n    },\n    \"path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The path to the exported report's raw data results. \"\n        }\n      ]\n    },\n    \"packaging\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportPackagingType\"\n        },\n        {\n          \"description\": \"<p> The type of build output artifact to create. Valid values include: </p> <ul> <li> <p> <code>NONE</code>: CodeBuild creates the raw data in the output bucket. This is the default if packaging is not specified. </p> </li> <li> <p> <code>ZIP</code>: CodeBuild creates a ZIP file with the raw data in the output bucket. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"encryptionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n \
  \       },\n        {\n          \"description\": \" The encryption key for the report's encrypted raw data. \"\n        }\n      ]\n    },\n    \"encryptionDisabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WrapperBoolean\"\n        },\n        {\n          \"description\": \" A boolean value that specifies if the results of a report are encrypted. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-s3-report-export-config-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: S3ReportExportConfig
---
