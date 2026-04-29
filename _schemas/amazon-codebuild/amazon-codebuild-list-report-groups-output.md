---
description: ListReportGroupsOutput schema from Amazon CodeBuild
layout: schema
name: ListReportGroupsOutput
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: reportGroups
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-report-groups-output-schema.json
slug: amazon-codebuild-list-report-groups-output
source_filename: amazon-codebuild-list-report-groups-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-report-groups-output-schema.json\",\n  \"title\": \"ListReportGroupsOutput\",\n  \"description\": \"ListReportGroupsOutput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" During a previous call, the maximum number of items that can be returned is the value specified in <code>maxResults</code>. If there more items in the list, then a unique string called a <i>nextToken</i> is returned. To get the next batch of items in the list, call this operation again, adding the next token to the call. To get all of the items in the list, keep calling this operation with each subsequent next token that is returned,\
  \ until no more next tokens are returned. \"\n        }\n      ]\n    },\n    \"reportGroups\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReportGroupArns\"\n        },\n        {\n          \"description\": \" The list of ARNs for the report groups in the current Amazon Web Services account. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-report-groups-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListReportGroupsOutput
---
