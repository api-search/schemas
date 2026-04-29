---
description: A custom action to use in stateless rule actions settings. This is used in <a>CustomAction</a>.
layout: schema
name: ActionDefinition
properties_list:
- description: ''
  name: PublishMetricAction
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-action-definition-schema.json
slug: openapi-action-definition
source_filename: openapi-action-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-action-definition-schema.json\",\n  \"title\": \"ActionDefinition\",\n  \"description\": \"A custom action to use in stateless rule actions settings. This is used in <a>CustomAction</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PublishMetricAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublishMetricAction\"\n        },\n        {\n          \"description\": \"<p>Stateless inspection criteria that publishes the specified metrics to Amazon CloudWatch for the matching packet. This setting defines a CloudWatch dimension value to be published.</p> <p>You can pair this custom action with any of the standard stateless rule actions. For example, you could pair this in a rule action with the standard action that forwards the packet for stateful\
  \ inspection. Then, when a packet matches the rule, Network Firewall publishes metrics for the packet and forwards it. </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-action-definition-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ActionDefinition
---
