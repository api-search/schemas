---
description: PutTelemetryRecordsRequest schema from Amazon X-Ray API
layout: schema
name: PutTelemetryRecordsRequest
properties_list:
- description: ''
  name: TelemetryRecords
  type: object
- description: ''
  name: EC2InstanceId
  type: object
- description: ''
  name: Hostname
  type: object
- description: ''
  name: ResourceARN
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-put-telemetry-records-request-schema.json
slug: xray-put-telemetry-records-request
source_filename: xray-put-telemetry-records-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"TelemetryRecords\"\n  ],\n  \"title\": \"PutTelemetryRecordsRequest\",\n  \"properties\": {\n    \"TelemetryRecords\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TelemetryRecordList\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"EC2InstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EC2InstanceId\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"Hostname\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Hostname\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-telemetry-records-request-schema.json\",\n  \"description\": \"PutTelemetryRecordsRequest schema from Amazon X-Ray API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-put-telemetry-records-request-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: PutTelemetryRecordsRequest
---
