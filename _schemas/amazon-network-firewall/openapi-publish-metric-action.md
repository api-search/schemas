---
description: Stateless inspection criteria that publishes the specified metrics to Amazon CloudWatch for the matching packet. This setting defines a CloudWatch dimension value to be published.
layout: schema
name: PublishMetricAction
properties_list:
- description: ''
  name: Dimensions
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-publish-metric-action-schema.json
slug: openapi-publish-metric-action
source_filename: openapi-publish-metric-action-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-publish-metric-action-schema.json\",\n  \"title\": \"PublishMetricAction\",\n  \"description\": \"Stateless inspection criteria that publishes the specified metrics to Amazon CloudWatch for the matching packet. This setting defines a CloudWatch dimension value to be published.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Dimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Dimensions\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Dimensions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-publish-metric-action-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: PublishMetricAction
---
