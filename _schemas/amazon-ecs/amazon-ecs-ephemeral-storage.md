---
description: ''
layout: schema
name: EphemeralStorage
properties_list:
- description: The total amount, in GiB, of ephemeral storage to set for the task. The minimum supported value is 21 GiB and the maximum supported value is 200 GiB.
  name: sizeInGiB
  type: integer
provider_name: Amazon ECS
provider_slug: amazon-ecs
schema_file: json-schema/amazon-ecs-ephemeral-storage-schema.json
slug: amazon-ecs-ephemeral-storage
source_filename: amazon-ecs-ephemeral-storage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EphemeralStorage\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sizeInGiB\": {\n      \"type\": \"integer\",\n      \"description\": \"The total amount, in GiB, of ephemeral storage to set for the task. The minimum supported value is 21 GiB and the maximum supported value is 200 GiB.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ecs/refs/heads/main/json-schema/amazon-ecs-ephemeral-storage-schema.json
tags:
- Amazon
- Aws
- Containers
- Docker
- Ecs
- Orchestration
title: EphemeralStorage
---
