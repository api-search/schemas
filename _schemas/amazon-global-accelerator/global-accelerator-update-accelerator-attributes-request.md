---
description: UpdateAcceleratorAttributesRequest schema from Amazon Global Accelerator API
layout: schema
name: UpdateAcceleratorAttributesRequest
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
- description: ''
  name: FlowLogsEnabled
  type: object
- description: ''
  name: FlowLogsS3Bucket
  type: object
- description: ''
  name: FlowLogsS3Prefix
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-accelerator-attributes-request-schema.json
slug: global-accelerator-update-accelerator-attributes-request
source_filename: global-accelerator-update-accelerator-attributes-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-accelerator-attributes-request-schema.json\",\n  \"title\": \"UpdateAcceleratorAttributesRequest\",\n  \"description\": \"UpdateAcceleratorAttributesRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accelerator that you want to update.\"\n        }\n      ]\n    },\n    \"FlowLogsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Update whether flow logs are enabled. The default value is false. If the value\
  \ is true, <code>FlowLogsS3Bucket</code> and <code>FlowLogsS3Prefix</code> must be specified.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/monitoring-global-accelerator.flow-logs.html\\\">Flow Logs</a> in the <i>Global Accelerator Developer Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"FlowLogsS3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket for the flow logs. Attribute is required if <code>FlowLogsEnabled</code> is <code>true</code>. The bucket must exist and have a bucket policy that grants Global Accelerator permission to write to the bucket.\"\n        }\n      ]\n    },\n    \"FlowLogsS3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>Update the prefix for the location in\
  \ the Amazon S3 bucket for the flow logs. Attribute is required if <code>FlowLogsEnabled</code> is <code>true</code>. </p> <p>If you specify slash (/) for the S3 bucket prefix, the log file bucket folder structure will include a double slash (//), like the following:</p> <p>s3-bucket_name//AWSLogs/aws_account_id</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AcceleratorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-accelerator-attributes-request-schema.json
tags:
- Availability
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateAcceleratorAttributesRequest
---
