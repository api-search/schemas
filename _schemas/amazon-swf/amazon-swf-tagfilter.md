---
description: Used to filter the workflow executions in visibility APIs based on a tag.
layout: schema
name: TagFilter
properties_list:
- description: ''
  name: tag
  type: object
provider_name: Amazon Simple Workflow Service
provider_slug: amazon-swf
schema_file: json-schema/amazon-swf-tagfilter-schema.json
slug: amazon-swf-tagfilter
source_filename: amazon-swf-tagfilter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"tag\"\n  ],\n  \"properties\": {\n    \"tag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tag\"\n        },\n        {\n          \"description\": \"<p> Specifies the tag that must be associated with the execution for it to meet the filter criteria.</p> <p>Tags may only contain unicode letters, digits, whitespace, or these symbols: <code>_ . : / = + - @</code>.</p>\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Used to filter the workflow executions in visibility APIs based on a tag.\",\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TagFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-swf/refs/heads/main/json-schema/amazon-swf-tagfilter-schema.json
tags:
- Automation
- Task Coordination
- Workflow
title: TagFilter
---
