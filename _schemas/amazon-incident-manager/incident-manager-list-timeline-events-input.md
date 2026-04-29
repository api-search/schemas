---
description: ListTimelineEventsInput schema
layout: schema
name: ListTimelineEventsInput
properties_list:
- description: ''
  name: filters
  type: object
- description: ''
  name: incidentRecordArn
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Incident Manager
provider_slug: amazon-incident-manager
schema_file: json-schema/incident-manager-list-timeline-events-input-schema.json
slug: incident-manager-list-timeline-events-input
source_filename: incident-manager-list-timeline-events-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-timeline-events-input-schema.json\",\n  \"title\": \"ListTimelineEventsInput\",\n  \"description\": \"ListTimelineEventsInput schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterList\"\n        },\n        {\n          \"description\": \"<p>Filters the timeline events based on the provided conditional values. You can filter timeline events with the following keys:</p> <ul> <li> <p> <code>eventTime</code> </p> </li> <li> <p> <code>eventType</code> </p> </li> </ul> <p>Note the following when deciding how to use Filters:</p> <ul> <li> <p>If you don't specify a Filter, the response includes all timeline events.</p> </li> <li> <p>If you specify more than one filter in a single\
  \ request, the response returns timeline events that match all filters.</p> </li> <li> <p>If you specify a filter with more than one value, the response returns timeline events that match any of the values provided.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"incidentRecordArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the incident that includes the timeline event.\"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"The maximum number of results per page.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The pagination token to continue to the next page of results.\"\n \
  \       }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimelineEventSort\"\n        },\n        {\n          \"description\": \"Sort timeline events by the specified key value pair.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\n        },\n        {\n          \"description\": \"Sorts the order of timeline events by the value specified in the <code>sortBy</code> field.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"incidentRecordArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-incident-manager/refs/heads/main/json-schema/incident-manager-list-timeline-events-input-schema.json
tags:
- Automation
- AWS
- DevOps
- Incident Management
- Operations
title: ListTimelineEventsInput
---
