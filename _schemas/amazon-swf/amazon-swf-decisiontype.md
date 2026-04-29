---
description: ''
layout: schema
name: DecisionType
properties_list: []
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-decisiontype-schema.json
slug: amazon-swf-decisiontype
source_json: "{\n  \"type\": \"string\",\n  \"enum\": [\n    \"ScheduleActivityTask\",\n    \"RequestCancelActivityTask\",\n    \"CompleteWorkflowExecution\",\n    \"FailWorkflowExecution\",\n    \"CancelWorkflowExecution\",\n    \"ContinueAsNewWorkflowExecution\",\n    \"RecordMarker\",\n    \"StartTimer\",\n    \"CancelTimer\",\n    \"SignalExternalWorkflowExecution\",\n    \"RequestCancelExternalWorkflowExecution\",\n    \"StartChildWorkflowExecution\",\n    \"ScheduleLambdaFunction\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DecisionType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-decisiontype-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DecisionType
---
