---
description: RoutedResources schema
layout: schema
name: RoutedResources
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-routed-resources-schema.json
slug: iot-events-routed-resources
source_filename: iot-events-routed-resources-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-routed-resources-schema.json\",\n  \"title\": \"RoutedResources\",\n  \"description\": \"RoutedResources schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"name\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ResourceName\"\n          },\n          {\n            \"description\": \" The name of the routed resource. \"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AmazonResourceName\"\n          },\n          {\n            \"description\": \" The ARN of the routed resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names\
  \ (ARNs)</a> in the <i>AWS General Reference</i>. \"\n          }\n        ]\n      }\n    },\n    \"description\": \" Contains information about the routed resource. \"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-routed-resources-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: RoutedResources
---
