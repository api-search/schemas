---
description: <p>Elastic Transcoder returns a warning if the resources used by your pipeline are not in the same region as the pipeline.</p> <p>Using resources in the same region, such as your Amazon S3 buckets, Amazon SNS notification topics, and AWS KMS key, reduces processing time and prevents cross-regional charges.</p>
layout: schema
name: Warning
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-warning-schema.json
slug: amazon-elastic-transcoder-warning
source_filename: amazon-elastic-transcoder-warning-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-warning-schema.json\",\n  \"title\": \"Warning\",\n  \"description\": \"<p>Elastic Transcoder returns a warning if the resources used by your pipeline are not in the same region as the pipeline.</p> <p>Using resources in the same region, such as your Amazon S3 buckets, Amazon SNS notification topics, and AWS KMS key, reduces processing time and prevents cross-regional charges.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The code of the cross-regional warning.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n  \
  \      {\n          \"description\": \"<p>The message explaining what resources are in a different region from the pipeline.</p> <note> <p>AWS KMS keys must be in the same region as the pipeline.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-warning-schema.json
tags:
- Amazon Web Services
- Media
- Transcoding
- Video
title: Warning
---
