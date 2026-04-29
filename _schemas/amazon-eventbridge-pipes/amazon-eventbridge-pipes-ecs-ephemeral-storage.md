---
description: <p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href="https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>This parameter is only supported for tasks hosted on Fargate using Linux platform version <code>1.4.0</code> or later. This parameter is not supported for Windows containers on Fargate.</p> </note>
layout: schema
name: EcsEphemeralStorage
properties_list:
- description: ''
  name: sizeInGiB
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-ecs-ephemeral-storage-schema.json
slug: amazon-eventbridge-pipes-ecs-ephemeral-storage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-ephemeral-storage-schema.json\",\n  \"title\": \"EcsEphemeralStorage\",\n  \"description\": \"<p>The amount of ephemeral storage to allocate for the task. This parameter is used to expand the total amount of ephemeral storage available, beyond the default amount, for tasks hosted on Fargate. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/userguide/using_data_volumes.html\\\">Fargate task storage</a> in the <i>Amazon ECS User Guide for Fargate</i>.</p> <note> <p>This parameter is only supported for tasks hosted on Fargate using Linux platform version <code>1.4.0</code> or later. This parameter is not supported for Windows containers on Fargate.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sizeInGiB\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemeralStorageSize\"\n        },\n        {\n          \"description\": \"The total amount, in GiB, of ephemeral storage to set for the task. The minimum supported value is <code>21</code> GiB and the maximum supported value is <code>200</code> GiB.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"sizeInGiB\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-ecs-ephemeral-storage-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: EcsEphemeralStorage
---
