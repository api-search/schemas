---
description: Details about an instance refresh rollback.
layout: schema
name: RollbackDetails
properties_list:
- description: ''
  name: RollbackReason
  type: object
- description: ''
  name: RollbackStartTime
  type: object
- description: ''
  name: PercentageCompleteOnRollback
  type: object
- description: ''
  name: InstancesToUpdateOnRollback
  type: object
- description: ''
  name: ProgressDetailsOnRollback
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-rollback-details-schema.json
slug: ec2-auto-scaling-rollback-details
source_filename: ec2-auto-scaling-rollback-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-rollback-details-schema.json\",\n  \"title\": \"RollbackDetails\",\n  \"description\": \"Details about an instance refresh rollback.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RollbackReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1023\"\n        },\n        {\n          \"description\": \"The reason for this instance refresh rollback (for example, whether a manual or automatic rollback was initiated).\"\n        }\n      ]\n    },\n    \"RollbackStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time at which the rollback began.\"\n        }\n      ]\n    },\n    \"PercentageCompleteOnRollback\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntPercent\"\n        },\n        {\n          \"description\": \"Indicates the value of <code>PercentageComplete</code> at the time the rollback started.\"\n        }\n      ]\n    },\n    \"InstancesToUpdateOnRollback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstancesToUpdate\"\n        },\n        {\n          \"description\": \"Indicates the value of <code>InstancesToUpdate</code> at the time the rollback started.\"\n        }\n      ]\n    },\n    \"ProgressDetailsOnRollback\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRefreshProgressDetails\"\n        },\n        {\n          \"description\": \"Reports progress on replacing instances in an Auto Scaling group that has a warm pool. This includes separate details for instances in the warm pool and instances in the Auto Scaling group (the live pool).\"\n        }\n      ]\n \
  \   }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-rollback-details-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: RollbackDetails
---
