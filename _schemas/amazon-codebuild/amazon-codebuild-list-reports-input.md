---
description: ListReportsInput schema from Amazon CodeBuild
layout: schema
name: ListReportsInput
properties_list:
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: filter
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-reports-input-schema.json
slug: amazon-codebuild-list-reports-input
source_filename: amazon-codebuild-list-reports-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-reports-input-schema.json\",\n  \"title\": \"ListReportsInput\",\n  \"description\": \"ListReportsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrderType\"\n        },\n        {\n          \"description\": \"<p> Specifies the sort order for the list of returned reports. Valid values are: </p> <ul> <li> <p> <code>ASCENDING</code>: return reports in chronological order based on their creation date. </p> </li> <li> <p> <code>DESCENDING</code>: return reports in the reverse chronological order based on their creation date. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \" During a previous call, the maximum number of items that can be returned is the value specified in <code>maxResults</code>. If there more items in the list, then a unique string called a <i>nextToken</i> is returned. To get the next batch of items in the list, call this operation again, adding the next token to the call. To get all of the items in the list, keep calling this operation with each subsequent next token that is returned, until no more next tokens are returned. \"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \" The maximum number of paginated reports returned per response. Use <code>nextToken</code> to iterate pages in the list of returned <code>Report</code> objects. The default value is 100. \"\n        }\n      ]\n    },\n    \"filter\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/ReportFilter\"\n        },\n        {\n          \"description\": \" A <code>ReportFilter</code> object used to filter the returned reports. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-reports-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListReportsInput
---
