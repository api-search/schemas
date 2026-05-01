---
description: ListSharedReportGroupsInput schema from Amazon CodeBuild
layout: schema
name: ListSharedReportGroupsInput
properties_list:
- description: ''
  name: sortOrder
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
provider_name: Amazon CodeBuild
provider_slug: amazon-codebuild
schema_file: json-schema/amazon-codebuild-list-shared-report-groups-input-schema.json
slug: amazon-codebuild-list-shared-report-groups-input
source_filename: amazon-codebuild-list-shared-report-groups-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-shared-report-groups-input-schema.json\",\n  \"title\": \"ListSharedReportGroupsInput\",\n  \"description\": \"ListSharedReportGroupsInput schema from Amazon CodeBuild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrderType\"\n        },\n        {\n          \"description\": \"<p>The order in which to list shared report groups. Valid values include:</p> <ul> <li> <p> <code>ASCENDING</code>: List in ascending order.</p> </li> <li> <p> <code>DESCENDING</code>: List in descending order.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SharedResourceSortByType\"\n        },\n        {\n    \
  \      \"description\": \"<p> The criterion to be used to list report groups shared with the current Amazon Web Services account or user. Valid values include: </p> <ul> <li> <p> <code>ARN</code>: List based on the ARN. </p> </li> <li> <p> <code>MODIFIED_TIME</code>: List based on when information about the shared report group was last changed. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" During a previous call, the maximum number of items that can be returned is the value specified in <code>maxResults</code>. If there more items in the list, then a unique string called a <i>nextToken</i> is returned. To get the next batch of items in the list, call this operation again, adding the next token to the call. To get all of the items in the list, keep calling this operation with each subsequent next token that is returned, until no\
  \ more next tokens are returned. \"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \" The maximum number of paginated shared report groups per response. Use <code>nextToken</code> to iterate pages in the list of returned <code>ReportGroup</code> objects. The default value is 100. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codebuild/refs/heads/main/json-schema/amazon-codebuild-list-shared-report-groups-input-schema.json
tags:
- Amazon
- CI/CD
- Build
- Continuous Integration
- DevOps
- Testing
title: ListSharedReportGroupsInput
---
