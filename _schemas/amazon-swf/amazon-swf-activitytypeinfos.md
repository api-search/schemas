---
description: Contains a paginated list of activity type information structures.
layout: schema
name: ActivityTypeInfos
properties_list:
- description: ''
  name: typeInfos
  type: object
- description: ''
  name: nextPageToken
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-activitytypeinfos-schema.json
slug: amazon-swf-activitytypeinfos
source_filename: amazon-swf-activitytypeinfos-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"typeInfos\"\n  ],\n  \"properties\": {\n    \"typeInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActivityTypeInfoList\"\n        },\n        {\n          \"description\": \"List of activity type information.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If a <code>NextPageToken</code> was returned by a previous call, there are more results available. To retrieve the next page of results, make the call again using the returned token in <code>nextPageToken</code>. Keep all other arguments unchanged.</p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains a paginated list of activity type information structures.\"\
  ,\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ActivityTypeInfos\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-activitytypeinfos-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: ActivityTypeInfos
---
