---
description: Represents information about incompatibility.
layout: schema
name: IncompatibilityMessage
properties_list:
- description: ''
  name: message
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-incompatibility-message-schema.json
slug: amazon-device-farm-incompatibility-message
source_filename: amazon-device-farm-incompatibility-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-incompatibility-message-schema.json\",\n  \"title\": \"IncompatibilityMessage\",\n  \"description\": \"Represents information about incompatibility.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A message about the incompatibility.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceAttribute\"\n        },\n        {\n          \"description\": \"<p>The type of incompatibility.</p> <p>Allowed values include:</p> <ul> <li> <p>ARN</p> </li> <li> <p>FORM_FACTOR (for example, phone or tablet)</p> </li> <li> <p>MANUFACTURER</p> </li> <li> <p>PLATFORM (for\
  \ example, Android or iOS)</p> </li> <li> <p>REMOTE_ACCESS_ENABLED</p> </li> <li> <p>APPIUM_VERSION</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-incompatibility-message-schema.json
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
title: IncompatibilityMessage
---
