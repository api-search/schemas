---
description: Represents the metadata of a device offering.
layout: schema
name: Offering
properties_list:
- description: ''
  name: id
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: recurringCharges
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-offering-schema.json
slug: amazon-device-farm-offering
source_filename: amazon-device-farm-offering-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-offering-schema.json\",\n  \"title\": \"Offering\",\n  \"description\": \"Represents the metadata of a device offering.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OfferingIdentifier\"\n        },\n        {\n          \"description\": \"The ID that corresponds to a device offering.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"A string that describes the offering.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OfferingType\"\n        },\n        {\n          \"description\"\
  : \"The type of offering (for example, <code>RECURRING</code>) for a device.\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevicePlatform\"\n        },\n        {\n          \"description\": \"The platform of the device (for example, <code>ANDROID</code> or <code>IOS</code>).\"\n        }\n      ]\n    },\n    \"recurringCharges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecurringCharges\"\n        },\n        {\n          \"description\": \"Specifies whether there are recurring charges for the offering.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-offering-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: Offering
---
