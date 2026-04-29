---
description: UpdateAcceleratorRequest schema from Amazon Global Accelerator API
layout: schema
name: UpdateAcceleratorRequest
properties_list:
- description: ''
  name: AcceleratorArn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: IpAddressType
  type: object
- description: ''
  name: Enabled
  type: object
provider_name: Amazon Global Accelerator
provider_slug: amazon-global-accelerator
schema_file: json-schema/global-accelerator-update-accelerator-request-schema.json
slug: global-accelerator-update-accelerator-request
source_filename: global-accelerator-update-accelerator-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-accelerator-request-schema.json\",\n  \"title\": \"UpdateAcceleratorRequest\",\n  \"description\": \"UpdateAcceleratorRequest schema from Amazon Global Accelerator API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcceleratorArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the accelerator to update.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\n        },\n        {\n          \"description\": \"The name of the accelerator. The name can have a maximum of 64 characters, must contain only alphanumeric characters, periods (.), or hyphens\
  \ (-), and must not begin or end with a hyphen or period.\"\n        }\n      ]\n    },\n    \"IpAddressType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpAddressType\"\n        },\n        {\n          \"description\": \"The IP address type that an accelerator supports. For a standard accelerator, the value can be IPV4 or DUAL_STACK.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericBoolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether an accelerator is enabled. The value is true or false. The default value is true. </p> <p>If the value is set to true, the accelerator cannot be deleted. If set to false, the accelerator can be deleted.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AcceleratorArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-global-accelerator/refs/heads/main/json-schema/global-accelerator-update-accelerator-request-schema.json
tags:
- Availability
- AWS
- CDN
- Global
- Load Balancing
- Networking
- Performance
title: UpdateAcceleratorRequest
---
