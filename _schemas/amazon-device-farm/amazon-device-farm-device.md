---
description: Represents a device type that an app is tested against.
layout: schema
name: Device
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: manufacturer
  type: object
- description: ''
  name: model
  type: object
- description: ''
  name: modelId
  type: object
- description: ''
  name: formFactor
  type: object
- description: ''
  name: platform
  type: object
- description: ''
  name: os
  type: object
- description: ''
  name: cpu
  type: object
- description: ''
  name: resolution
  type: object
- description: ''
  name: heapSize
  type: object
- description: ''
  name: memory
  type: object
- description: ''
  name: image
  type: object
- description: ''
  name: carrier
  type: object
- description: ''
  name: radio
  type: object
- description: ''
  name: remoteAccessEnabled
  type: object
- description: ''
  name: remoteDebugEnabled
  type: object
- description: ''
  name: fleetType
  type: object
- description: ''
  name: fleetName
  type: object
- description: ''
  name: instances
  type: object
- description: ''
  name: availability
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-device-schema.json
slug: amazon-device-farm-device
source_filename: amazon-device-farm-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"Represents a device type that an app is tested against.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The device's ARN.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The device's display name.\"\n        }\n      ]\n    },\n    \"manufacturer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's manufacturer name.\"\
  \n        }\n      ]\n    },\n    \"model\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's model name.\"\n        }\n      ]\n    },\n    \"modelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's model ID.\"\n        }\n      ]\n    },\n    \"formFactor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceFormFactor\"\n        },\n        {\n          \"description\": \"<p>The device's form factor.</p> <p>Allowed values include:</p> <ul> <li> <p>PHONE</p> </li> <li> <p>TABLET</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"platform\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DevicePlatform\"\n        },\n        {\n          \"description\": \"<p>The device's platform.</p> <p>Allowed values include:</p>\
  \ <ul> <li> <p>ANDROID</p> </li> <li> <p>IOS</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"os\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's operating system type.\"\n        }\n      ]\n    },\n    \"cpu\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CPU\"\n        },\n        {\n          \"description\": \"Information about the device's CPU.\"\n        }\n      ]\n    },\n    \"resolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Resolution\"\n        },\n        {\n          \"description\": \"The resolution of the device.\"\n        }\n      ]\n    },\n    \"heapSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The device's heap size, expressed in bytes.\"\n        }\n      ]\n    },\n    \"memory\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The device's total memory size, expressed in bytes.\"\n        }\n      ]\n    },\n    \"image\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's image name.\"\n        }\n      ]\n    },\n    \"carrier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's carrier.\"\n        }\n      ]\n    },\n    \"radio\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The device's radio.\"\n        }\n      ]\n    },\n    \"remoteAccessEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\"\
  : \"Specifies whether remote access has been enabled for the specified device.\"\n        }\n      ]\n    },\n    \"remoteDebugEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>This flag is set to <code>true</code> if remote debugging is enabled for the device.</p> <p>Remote debugging is <a href=\\\"https://docs.aws.amazon.com/devicefarm/latest/developerguide/history.html\\\">no longer supported</a>.</p>\"\n        }\n      ]\n    },\n    \"fleetType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of fleet to which this device belongs. Possible values are PRIVATE and PUBLIC.\"\n        }\n      ]\n    },\n    \"fleetName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the fleet\
  \ to which this device belongs.\"\n        }\n      ]\n    },\n    \"instances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceInstances\"\n        },\n        {\n          \"description\": \"The instances that belong to this device.\"\n        }\n      ]\n    },\n    \"availability\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceAvailability\"\n        },\n        {\n          \"description\": \"Indicates how likely a device is available for a test run. Currently available in the <a>ListDevices</a> and GetDevice API methods.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-device-schema.json
tags:
- Application Testing
- Device Testing
- Mobile Testing
- Quality Assurance
title: Device
---
