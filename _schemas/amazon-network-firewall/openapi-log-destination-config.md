---
description: <p>Defines where Network Firewall sends logs for the firewall for one log type. This is used in <a>LoggingConfiguration</a>. You can send each type of log to an Amazon S3 bucket, a CloudWatch log group, or a Kinesis Data Firehose delivery stream.</p> <p>Network Firewall generates logs for stateful rule groups. You can save alert and flow log types. The stateful rules engine records flow logs for all network traffic that it receives. It records alert logs for traffic that matches stateful rules that have the rule action set to <code>DROP</code> or <code>ALERT</code>. </p>
layout: schema
name: LogDestinationConfig
properties_list:
- description: ''
  name: LogType
  type: object
- description: ''
  name: LogDestinationType
  type: object
- description: ''
  name: LogDestination
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-log-destination-config-schema.json
slug: openapi-log-destination-config
source_filename: openapi-log-destination-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-log-destination-config-schema.json\",\n  \"title\": \"LogDestinationConfig\",\n  \"description\": \"<p>Defines where Network Firewall sends logs for the firewall for one log type. This is used in <a>LoggingConfiguration</a>. You can send each type of log to an Amazon S3 bucket, a CloudWatch log group, or a Kinesis Data Firehose delivery stream.</p> <p>Network Firewall generates logs for stateful rule groups. You can save alert and flow log types. The stateful rules engine records flow logs for all network traffic that it receives. It records alert logs for traffic that matches stateful rules that have the rule action set to <code>DROP</code> or <code>ALERT</code>. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogType\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/LogType\"\n        },\n        {\n          \"description\": \"The type of log to send. Alert logs report traffic that matches a <a>StatefulRule</a> with an action setting that sends an alert log message. Flow logs are standard network traffic flow logs. \"\n        }\n      ]\n    },\n    \"LogDestinationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogDestinationType\"\n        },\n        {\n          \"description\": \"The type of storage destination to send these logs to. You can send logs to an Amazon S3 bucket, a CloudWatch log group, or a Kinesis Data Firehose delivery stream.\"\n        }\n      ]\n    },\n    \"LogDestination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogDestinationMap\"\n        },\n        {\n          \"description\": \"<p>The named location for the logs, provided in a key:value mapping that is specific to the chosen destination type. </p> <ul> <li> <p>For\
  \ an Amazon S3 bucket, provide the name of the bucket, with key <code>bucketName</code>, and optionally provide a prefix, with key <code>prefix</code>. The following example specifies an Amazon S3 bucket named <code>DOC-EXAMPLE-BUCKET</code> and the prefix <code>alerts</code>: </p> <p> <code>\\\"LogDestination\\\": { \\\"bucketName\\\": \\\"DOC-EXAMPLE-BUCKET\\\", \\\"prefix\\\": \\\"alerts\\\" }</code> </p> </li> <li> <p>For a CloudWatch log group, provide the name of the CloudWatch log group, with key <code>logGroup</code>. The following example specifies a log group named <code>alert-log-group</code>: </p> <p> <code>\\\"LogDestination\\\": { \\\"logGroup\\\": \\\"alert-log-group\\\" }</code> </p> </li> <li> <p>For a Kinesis Data Firehose delivery stream, provide the name of the delivery stream, with key <code>deliveryStream</code>. The following example specifies a delivery stream named <code>alert-delivery-stream</code>: </p> <p> <code>\\\"LogDestination\\\": { \\\"deliveryStream\\\
  \": \\\"alert-delivery-stream\\\" }</code> </p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogType\",\n    \"LogDestinationType\",\n    \"LogDestination\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-log-destination-config-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: LogDestinationConfig
---
