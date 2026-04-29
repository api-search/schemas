---
description: Describes the point at which the application reads from the streaming source.
layout: schema
name: InputStartingPositionConfiguration
properties_list:
- description: ''
  name: InputStartingPosition
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-starting-position-configuration-schema.json
slug: amazon-managed-apache-flink-input-starting-position-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-starting-position-configuration-schema.json\",\n  \"title\": \"InputStartingPositionConfiguration\",\n  \"description\": \"Describes the point at which the application reads from the streaming source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputStartingPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputStartingPosition\"\n        },\n        {\n          \"description\": \"<p>The starting position on the stream.</p> <ul> <li> <p> <code>NOW</code> - Start reading just after the most recent record in the stream, and start at the request timestamp that the customer issued.</p> </li> <li> <p> <code>TRIM_HORIZON</code> - Start reading at the last untrimmed record in the stream, which is the oldest record\
  \ available in the stream. This option is not available for an Amazon Kinesis Data Firehose delivery stream.</p> </li> <li> <p> <code>LAST_STOPPED_POINT</code> - Resume reading from where the application last stopped reading.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-starting-position-configuration-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputStartingPositionConfiguration
---
