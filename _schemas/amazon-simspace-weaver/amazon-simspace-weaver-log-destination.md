---
description: The location where SimSpace Weaver sends simulation log data.
layout: schema
name: LogDestination
properties_list:
- description: ''
  name: CloudWatchLogsLogGroup
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-log-destination-schema.json
slug: amazon-simspace-weaver-log-destination
source_filename: amazon-simspace-weaver-log-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-log-destination-schema.json\",\n  \"title\": \"LogDestination\",\n  \"description\": \"The location where SimSpace Weaver sends simulation log data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudWatchLogsLogGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogsLogGroup\"\n        },\n        {\n          \"description\": \"An Amazon CloudWatch Logs log group that stores simulation log data. For more information about log groups, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Working-with-log-groups-and-streams.html\\\">Working with log groups and log streams</a> in the <i>Amazon CloudWatch Logs User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-log-destination-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: LogDestination
---
