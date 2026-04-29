---
description: UpdateGatewayInformationInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateGatewayInformationInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: GatewayName
  type: object
- description: ''
  name: GatewayTimezone
  type: object
- description: ''
  name: CloudWatchLogGroupARN
  type: object
- description: ''
  name: GatewayCapacity
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-gateway-information-input-schema.json
slug: amazon-storage-gateway-update-gateway-information-input
source_filename: amazon-storage-gateway-update-gateway-information-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-gateway-information-input-schema.json\",\n  \"title\": \"UpdateGatewayInformationInput\",\n  \"description\": \"UpdateGatewayInformationInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"GatewayName\": {\n      \"$ref\": \"#/components/schemas/GatewayName\"\n    },\n    \"GatewayTimezone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayTimezone\"\n        },\n        {\n          \"description\": \"A value that indicates the time zone of the gateway.\"\n        }\n      ]\n    },\n    \"CloudWatchLogGroupARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogGroupARN\"\
  \n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the Amazon CloudWatch log group that you want to use to monitor and log events in the gateway.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonCloudWatch/latest/logs/WhatIsCloudWatchLogs.html\\\">What is Amazon CloudWatch Logs?</a> </p>\"\n        }\n      ]\n    },\n    \"GatewayCapacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayCapacity\"\n        },\n        {\n          \"description\": \"Specifies the size of the gateway's metadata cache.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-gateway-information-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateGatewayInformationInput
---
