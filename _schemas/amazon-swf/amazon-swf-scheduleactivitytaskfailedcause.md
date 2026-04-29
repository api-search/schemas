---
description: ''
layout: schema
name: ScheduleActivityTaskFailedCause
properties_list: []
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-scheduleactivitytaskfailedcause-schema.json
slug: amazon-swf-scheduleactivitytaskfailedcause
source_json: "{\n  \"type\": \"string\",\n  \"enum\": [\n    \"ACTIVITY_TYPE_DEPRECATED\",\n    \"ACTIVITY_TYPE_DOES_NOT_EXIST\",\n    \"ACTIVITY_ID_ALREADY_IN_USE\",\n    \"OPEN_ACTIVITIES_LIMIT_EXCEEDED\",\n    \"ACTIVITY_CREATION_RATE_EXCEEDED\",\n    \"DEFAULT_SCHEDULE_TO_CLOSE_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_TASK_LIST_UNDEFINED\",\n    \"DEFAULT_SCHEDULE_TO_START_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_START_TO_CLOSE_TIMEOUT_UNDEFINED\",\n    \"DEFAULT_HEARTBEAT_TIMEOUT_UNDEFINED\",\n    \"OPERATION_NOT_PERMITTED\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ScheduleActivityTaskFailedCause\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-scheduleactivitytaskfailedcause-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: ScheduleActivityTaskFailedCause
---
