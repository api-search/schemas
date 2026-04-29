---
description: The container for the <a>EventTriggerDefinition$EventResourceARN</a>.
layout: schema
name: EventTriggerDefinition
properties_list:
- description: ''
  name: EventResourceARN
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-event-trigger-definition-schema.json
slug: amazon-snow-family-event-trigger-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-event-trigger-definition-schema.json\",\n  \"title\": \"EventTriggerDefinition\",\n  \"description\": \"The container for the <a>EventTriggerDefinition$EventResourceARN</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EventResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for any local Amazon S3 resource that is an Lambda function's event trigger associated with this job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-event-trigger-definition-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: EventTriggerDefinition
---
