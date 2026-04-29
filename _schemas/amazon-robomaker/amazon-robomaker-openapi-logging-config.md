---
description: The logging configuration.
layout: schema
name: LoggingConfig
properties_list:
- description: ''
  name: recordAllRosTopics
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-logging-config-schema.json
slug: amazon-robomaker-openapi-logging-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-logging-config-schema.json\",\n  \"title\": \"LoggingConfig\",\n  \"description\": \"The logging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recordAllRosTopics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoxedBoolean\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"<p>A boolean indicating whether to record all ROS topics.</p> <important> <p>This API is no longer supported and will throw an error if used.</p> </important>AWS RoboMaker is ending support for ROS software suite. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/software-support-policy.html.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-logging-config-schema.json
tags:
- AWS
- Robotics
- Simulation
title: LoggingConfig
---
