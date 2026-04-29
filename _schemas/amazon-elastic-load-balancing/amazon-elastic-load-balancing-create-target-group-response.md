---
description: Response from the CreateTargetGroup action
layout: schema
name: CreateTargetGroupResponse
properties_list:
- description: Information about the target group
  name: targetGroups
  type: array
provider_name: Amazon Elastic Load Balancing
provider_slug: amazon-elastic-load-balancing
schema_file: json-schema/amazon-elastic-load-balancing-create-target-group-response-schema.json
slug: amazon-elastic-load-balancing-create-target-group-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-target-group-response-schema.json\",\n  \"title\": \"CreateTargetGroupResponse\",\n  \"description\": \"Response from the CreateTargetGroup action\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"targetGroups\": {\n      \"type\": \"array\",\n      \"description\": \"Information about the target group\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TargetGroup\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-load-balancing/refs/heads/main/json-schema/amazon-elastic-load-balancing-create-target-group-response-schema.json
tags:
- Amazon Web Services
- AWS
- High Availability
- Load Balancing
- Networking
- Scalability
title: CreateTargetGroupResponse
---
