---
description: Paginated representation of a workflow history for a workflow execution. This is the up to date, complete and authoritative record of the events related to all tasks and events in the life of the workflow execution.
layout: schema
name: History
properties_list:
- description: ''
  name: events
  type: object
- description: ''
  name: nextPageToken
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-history-schema.json
slug: amazon-swf-history
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"events\"\n  ],\n  \"properties\": {\n    \"events\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HistoryEventList\"\n        },\n        {\n          \"description\": \"The list of history events.\"\n        }\n      ]\n    },\n    \"nextPageToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageToken\"\n        },\n        {\n          \"description\": \"<p>If a <code>NextPageToken</code> was returned by a previous call, there are more results available. To retrieve the next page of results, make the call again using the returned token in <code>nextPageToken</code>. Keep all other arguments unchanged.</p> <p>The configured <code>maximumPageSize</code> determines how many results can be returned in a single call.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Paginated representation of a workflow history for a workflow execution. This is the\
  \ up to date, complete and authoritative record of the events related to all tasks and events in the life of the workflow execution.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"History\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-history-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: History
---
