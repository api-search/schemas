---
description: Provides the details of the <code>MarkerRecorded</code> event.
layout: schema
name: MarkerRecordedEventAttributes
properties_list:
- description: ''
  name: markerName
  type: object
- description: ''
  name: details
  type: object
- description: ''
  name: decisionTaskCompletedEventId
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-markerrecordedeventattributes-schema.json
slug: amazon-swf-markerrecordedeventattributes
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"markerName\",\n    \"decisionTaskCompletedEventId\"\n  ],\n  \"properties\": {\n    \"markerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MarkerName\"\n        },\n        {\n          \"description\": \"The name of the marker.\"\n        }\n      ]\n    },\n    \"details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Data\"\n        },\n        {\n          \"description\": \"The details of the marker.\"\n        }\n      ]\n    },\n    \"decisionTaskCompletedEventId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventId\"\n        },\n        {\n          \"description\": \"The ID of the <code>DecisionTaskCompleted</code> event corresponding to the decision task that resulted in the <code>RecordMarker</code> decision that requested this marker. This information can be useful for diagnosing problems by tracing back the\
  \ chain of events leading up to this event.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Provides the details of the <code>MarkerRecorded</code> event.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"MarkerRecordedEventAttributes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-markerrecordedeventattributes-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: MarkerRecordedEventAttributes
---
