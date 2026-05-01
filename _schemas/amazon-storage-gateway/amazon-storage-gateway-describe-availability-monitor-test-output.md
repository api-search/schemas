---
description: DescribeAvailabilityMonitorTestOutput schema from Amazon Storage Gateway API
layout: schema
name: DescribeAvailabilityMonitorTestOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-availability-monitor-test-output-schema.json
slug: amazon-storage-gateway-describe-availability-monitor-test-output
source_filename: amazon-storage-gateway-describe-availability-monitor-test-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-availability-monitor-test-output-schema.json\",\n  \"title\": \"DescribeAvailabilityMonitorTestOutput\",\n  \"description\": \"DescribeAvailabilityMonitorTestOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AvailabilityMonitorTestStatus\"\n        },\n        {\n          \"description\": \"The status of the high availability monitoring test. If a test hasn't been performed, the value of this field is null.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n   \
  \     },\n        {\n          \"description\": \"The time the high availability monitoring test was started. If a test hasn't been performed, the value of this field is null.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-availability-monitor-test-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeAvailabilityMonitorTestOutput
---
