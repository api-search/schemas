---
description: BatchPutScheduledUpdateGroupActionAnswer schema from Auto Scaling
layout: schema
name: BatchPutScheduledUpdateGroupActionAnswer
properties_list:
- description: ''
  name: FailedScheduledUpdateGroupActions
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-batch-put-scheduled-update-group-action-answer-schema.json
slug: ec2-auto-scaling-batch-put-scheduled-update-group-action-answer
source_filename: ec2-auto-scaling-batch-put-scheduled-update-group-action-answer-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-batch-put-scheduled-update-group-action-answer-schema.json\",\n  \"title\": \"BatchPutScheduledUpdateGroupActionAnswer\",\n  \"description\": \"BatchPutScheduledUpdateGroupActionAnswer schema from Auto Scaling\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedScheduledUpdateGroupActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedScheduledUpdateGroupActionRequests\"\n        },\n        {\n          \"description\": \"The names of the scheduled actions that could not be created or updated, including an error message.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-batch-put-scheduled-update-group-action-answer-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: BatchPutScheduledUpdateGroupActionAnswer
---
