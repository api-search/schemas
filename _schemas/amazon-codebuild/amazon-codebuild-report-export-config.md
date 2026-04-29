---
description: Information about the location where the run of a report is exported.
layout: schema
name: ReportExportConfig
properties_list:
- description: ''
  name: exportConfigType
  type: object
- description: ''
  name: s3Destination
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-report-export-config-schema.json
slug: amazon-codebuild-report-export-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-export-config-schema.json\",\n  \"title\": \"ReportExportConfig\",\n  \"description\": \" Information about the location where the run of a report is exported. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportConfigType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportExportConfigType\"\n        },\n        {\n          \"description\": \"<p> The export configuration type. Valid values are: </p> <ul> <li> <p> <code>S3</code>: The report results are exported to an S3 bucket. </p> </li> <li> <p> <code>NO_EXPORT</code>: The report results are not exported. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"s3Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3ReportExportConfig\"\n    \
  \    },\n        {\n          \"description\": \" A <code>S3ReportExportConfig</code> object that contains information about the S3 bucket where the run of a report is exported. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-export-config-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ReportExportConfig
---
