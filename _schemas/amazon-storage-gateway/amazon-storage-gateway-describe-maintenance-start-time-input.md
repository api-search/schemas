---
description: A JSON object containing the Amazon Resource Name (ARN) of the gateway.
layout: schema
name: DescribeMaintenanceStartTimeInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-maintenance-start-time-input-schema.json
slug: amazon-storage-gateway-describe-maintenance-start-time-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-maintenance-start-time-input-schema.json\",\n  \"title\": \"DescribeMaintenanceStartTimeInput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the gateway.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  },\n  \"required\": [\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-maintenance-start-time-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeMaintenanceStartTimeInput
---
