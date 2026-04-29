---
description: Attributes of a custom routing accelerator.
layout: schema
name: CustomRoutingAcceleratorAttributes
properties_list:
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
schema_file: json-schema/global-accelerator-custom-routing-accelerator-attributes-schema.json
slug: global-accelerator-custom-routing-accelerator-attributes
source_filename: global-accelerator-custom-routing-accelerator-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-accelerator-attributes-schema.json\",\n  \"title\": \"CustomRoutingAcceleratorAttributes\",\n  \"description\": \"Attributes of a custom routing accelerator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlowLogsEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether flow logs are enabled. The default value is false. If the value is true, <code>FlowLogsS3Bucket</code> and <code>FlowLogsS3Prefix</code> must be specified.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/global-accelerator/latest/dg/monitoring-global-accelerator.flow-logs.html\\\">Flow logs</a> in the <i>Global Accelerator Developer Guide</i>.</p>\"\
  \n        }\n      ]\n    },\n    \"FlowLogsS3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the Amazon S3 bucket for the flow logs. Attribute is required if <code>FlowLogsEnabled</code> is <code>true</code>. The bucket must exist and have a bucket policy that grants Global Accelerator permission to write to the bucket.\"\n        }\n      ]\n    },\n    \"FlowLogsS3Prefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"<p>The prefix for the location in the Amazon S3 bucket for the flow logs. Attribute is required if <code>FlowLogsEnabled</code> is <code>true</code>.</p> <p>If you don\\u2019t specify a prefix, the flow logs are stored in the root of the bucket. If you specify slash (/) for the S3 bucket prefix, the log file bucket folder structure will include a double\
  \ slash (//), like the following:</p> <p>DOC-EXAMPLE-BUCKET//AWSLogs/aws_account_id</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-custom-routing-accelerator-attributes-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: CustomRoutingAcceleratorAttributes
---
