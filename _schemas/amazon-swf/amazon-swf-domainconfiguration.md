---
description: Contains the configuration settings of a domain.
layout: schema
name: DomainConfiguration
properties_list:
- description: ''
  name: workflowExecutionRetentionPeriodInDays
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-domainconfiguration-schema.json
slug: amazon-swf-domainconfiguration
source_filename: amazon-swf-domainconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"workflowExecutionRetentionPeriodInDays\"\n  ],\n  \"properties\": {\n    \"workflowExecutionRetentionPeriodInDays\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DurationInDays\"\n        },\n        {\n          \"description\": \"The retention period for workflow executions in this domain.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains the configuration settings of a domain.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"DomainConfiguration\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-domainconfiguration-schema.json
tags:
- Automation
- AWS
- Task Coordination
- Workflow
title: DomainConfiguration
---
