---
description: Placeholder documentation for UpdateInputDeviceResponse
layout: schema
name: UpdateInputDeviceResponse
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: ConnectionState
  type: object
- description: ''
  name: DeviceSettingsSyncState
  type: object
- description: ''
  name: DeviceUpdateStatus
  type: object
- description: ''
  name: HdDeviceSettings
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: MacAddress
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: NetworkSettings
  type: object
- description: ''
  name: SerialNumber
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: UhdDeviceSettings
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-update-input-device-response-schema.json
slug: medialive-api-update-input-device-response
source_filename: medialive-api-update-input-device-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-device-response-schema.json\",\n  \"title\": \"UpdateInputDeviceResponse\",\n  \"description\": \"Placeholder documentation for UpdateInputDeviceResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The unique ARN of the input device.\"\n        }\n      ]\n    },\n    \"ConnectionState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceConnectionState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"connectionState\"\n          },\n          \"description\": \"The state of the connection between\
  \ the input device and AWS.\"\n        }\n      ]\n    },\n    \"DeviceSettingsSyncState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceSettingsSyncState\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deviceSettingsSyncState\"\n          },\n          \"description\": \"The status of the action to synchronize the device configuration. If you change the configuration of the input device (for example, the maximum bitrate), MediaLive sends the new data to the device. The device might not update itself immediately. SYNCED means the device has updated its configuration. SYNCING means that it has not updated its configuration.\"\n        }\n      ]\n    },\n    \"DeviceUpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceUpdateStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deviceUpdateStatus\"\n          },\n          \"description\": \"The status of software\
  \ on the input device.\"\n        }\n      ]\n    },\n    \"HdDeviceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceHdSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hdDeviceSettings\"\n          },\n          \"description\": \"Settings that describe an input device that is type HD.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The unique ID of the input device.\"\n        }\n      ]\n    },\n    \"MacAddress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"macAddress\"\n          },\n          \"description\": \"The network MAC address of the input device.\"\n        }\n      ]\n    },\n  \
  \  \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"name\"\n          },\n          \"description\": \"A name that you specify for the input device.\"\n        }\n      ]\n    },\n    \"NetworkSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceNetworkSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"networkSettings\"\n          },\n          \"description\": \"The network settings for the input device.\"\n        }\n      ]\n    },\n    \"SerialNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"serialNumber\"\n          },\n          \"description\": \"The unique serial number of the input device.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/InputDeviceType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"The type of the input device.\"\n        }\n      ]\n    },\n    \"UhdDeviceSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputDeviceUhdSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"uhdDeviceSettings\"\n          },\n          \"description\": \"Settings that describe an input device that is type UHD.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"tags\"\n          },\n          \"description\": \"A collection of key-value pairs.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-update-input-device-response-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: UpdateInputDeviceResponse
---
