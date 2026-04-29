---
description: ''
layout: schema
name: VisibilityConfig
properties_list:
- description: ''
  name: SampledRequestsEnabled
  type: boolean
- description: ''
  name: CloudWatchMetricsEnabled
  type: boolean
- description: ''
  name: MetricName
  type: string
provider_name: Amazon WAF
provider_slug: amazon-waf
schema_file: json-schema/amazon-waf-visibility-config-schema.json
slug: amazon-waf-visibility-config
source_filename: amazon-waf-visibility-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SampledRequestsEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"CloudWatchMetricsEnabled\": {\n      \"type\": \"boolean\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"SampledRequestsEnabled\",\n    \"CloudWatchMetricsEnabled\",\n    \"MetricName\"\n  ],\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"VisibilityConfig\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-waf/refs/heads/main/json-schema/amazon-waf-visibility-config-schema.json
tags:
- AWS
- Bot Management
- Ddos Protection
- Security
- WAF
- Web Application Firewall
title: VisibilityConfig
---
