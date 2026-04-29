---
description: TimestampString schema from Amazon Lookout for Metrics API
layout: schema
name: TimestampString
properties_list: []
provider_name: Amazon Lookout for Metrics
provider_slug: amazon-lookout-for-metrics
schema_file: json-schema/amazon-lookout-for-metrics-timestamp-string-schema.json
slug: amazon-lookout-for-metrics-timestamp-string
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-timestamp-string-schema.json\",\n  \"title\": \"TimestampString\",\n  \"description\": \"TimestampString schema from Amazon Lookout for Metrics API\",\n  \"type\": \"string\",\n  \"pattern\": \"^([12]\\\\d{3})-(1[0-2]|0[1-9])-(0[1-9]|[12]\\\\d|3[01])T([01]\\\\d|2[0-3]):([0-5]\\\\d):([0-5]\\\\d)(Z|(\\\\+|\\\\-)(0\\\\d|1[0-2]):([0-5]\\\\d)(\\\\[[[:alnum:]\\\\/\\\\_]+\\\\])?)$\",\n  \"maxLength\": 60\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lookout-for-metrics/refs/heads/main/json-schema/amazon-lookout-for-metrics-timestamp-string-schema.json
tags:
- Anomaly Detection
- AWS
- Business Intelligence
- Machine Learning
- Metrics
- Monitoring
title: TimestampString
---
