---
description: A series of reports. Each report contains information about the results from running a series of test cases. You specify the test cases for a report group in the buildspec for a build project using one or more paths to the test case files.
layout: schema
name: ReportGroup
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: exportConfig
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: lastModified
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-report-group-schema.json
slug: amazon-codebuild-report-group
source_filename: amazon-codebuild-report-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-group-schema.json\",\n  \"title\": \"ReportGroup\",\n  \"description\": \"A series of reports. Each report contains information about the results from running a series of test cases. You specify the test cases for a report group in the buildspec for a build project using one or more paths to the test case files. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The ARN of the <code>ReportGroup</code>. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupName\"\n        },\n        {\n          \"description\": \"The name of the <code>ReportGroup</code>.\
  \ \"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportType\"\n        },\n        {\n          \"description\": \"<p>The type of the <code>ReportGroup</code>. This can be one of the following values:</p> <dl> <dt>CODE_COVERAGE</dt> <dd> <p>The report group contains code coverage reports.</p> </dd> <dt>TEST</dt> <dd> <p>The report group contains test reports.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"exportConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportExportConfig\"\n        },\n        {\n          \"description\": \"Information about the destination where the raw data of this <code>ReportGroup</code> is exported. \"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time this <code>ReportGroup</code> was\
  \ created. \"\n        }\n      ]\n    },\n    \"lastModified\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time this <code>ReportGroup</code> was last modified. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"<p>A list of tag key and value pairs associated with this report group. </p> <p>These tags are available for use by Amazon Web Services services that support CodeBuild report group tags.</p>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupStatusType\"\n        },\n        {\n          \"description\": \"<p>The status of the report group. This property is read-only.</p> <p>This can be one of the following values:</p> <dl> <dt>ACTIVE</dt> <dd> <p>The\
  \ report group is active.</p> </dd> <dt>DELETING</dt> <dd> <p>The report group is in the process of being deleted.</p> </dd> </dl>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-report-group-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ReportGroup
---
