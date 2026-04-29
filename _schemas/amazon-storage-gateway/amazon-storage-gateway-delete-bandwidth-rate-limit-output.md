---
description: A JSON object containing the Amazon Resource Name (ARN) of the gateway whose bandwidth rate information was deleted.
layout: schema
name: DeleteBandwidthRateLimitOutput
properties_list:
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-bandwidth-rate-limit-output-schema.json
slug: amazon-storage-gateway-delete-bandwidth-rate-limit-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-bandwidth-rate-limit-output-schema.json\",\n  \"title\": \"DeleteBandwidthRateLimitOutput\",\n  \"description\": \"A JSON object containing the Amazon Resource Name (ARN) of the gateway whose bandwidth rate information was deleted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-bandwidth-rate-limit-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteBandwidthRateLimitOutput
---
