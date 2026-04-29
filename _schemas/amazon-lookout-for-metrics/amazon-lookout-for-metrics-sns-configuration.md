---
description: Contains information about the SNS topic to which you want to send your alerts and the IAM role that has access to that topic.
layout: schema
name: SNSConfiguration
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SnsTopicArn
  type: object
- description: ''
  name: SnsFormat
  type: object
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-sns-configuration-schema.json
slug: amazon-lookout-for-metrics-sns-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-sns-configuration-schema.json\",\n  \"title\": \"SNSConfiguration\",\n  \"description\": \"Contains information about the SNS topic to which you want to send your alerts and the IAM role that has access to that topic.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM role that has access to the target SNS topic.\"\n        }\n      ]\n    },\n    \"SnsTopicArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The ARN of the target SNS topic.\"\n        }\n      ]\n    },\n    \"SnsFormat\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/SnsFormat\"\n        },\n        {\n          \"description\": \"<p>The format of the SNS topic.</p> <ul> <li> <p> <code>JSON</code> \\u2013 Send JSON alerts with an anomaly ID and a link to the anomaly detail page. This is the default.</p> </li> <li> <p> <code>LONG_TEXT</code> \\u2013 Send human-readable alerts with information about the impacted timeseries and a link to the anomaly detail page. We recommend this for email.</p> </li> <li> <p> <code>SHORT_TEXT</code> \\u2013 Send human-readable alerts with a link to the anomaly detail page. We recommend this for SMS.</p> </li> </ul>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RoleArn\",\n    \"SnsTopicArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-sns-configuration-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: SNSConfiguration
---
