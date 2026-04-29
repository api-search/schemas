---
description: The Amazon CloudWatch Logs log group for the simulation. For more information about log groups, see <a href="https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Working-with-log-groups-and-streams.html">Working with log groups and log streams</a> in the <i>Amazon CloudWatch Logs User Guide</i>.
layout: schema
name: CloudWatchLogsLogGroup
properties_list:
- description: ''
  name: LogGroupArn
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-cloud-watch-logs-log-group-schema.json
slug: amazon-simspace-weaver-cloud-watch-logs-log-group
source_filename: amazon-simspace-weaver-cloud-watch-logs-log-group-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-cloud-watch-logs-log-group-schema.json\",\n  \"title\": \"CloudWatchLogsLogGroup\",\n  \"description\": \"The Amazon CloudWatch Logs log group for the simulation. For more information about log groups, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Working-with-log-groups-and-streams.html\\\">Working with log groups and log streams</a> in the <i>Amazon CloudWatch Logs User Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon CloudWatch Logs log group for the simulation. For more information about ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\
  \">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>. For more information about log groups, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/Working-with-log-groups-and-streams.html\\\">Working with log groups and log streams</a> in the <i>Amazon CloudWatch Logs User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-cloud-watch-logs-log-group-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: CloudWatchLogsLogGroup
---
