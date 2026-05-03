---
description: Schema for a Samsara driver entity as returned by the Samsara REST API. Represents a commercial vehicle driver managed in the Samsara platform.
layout: schema
name: Samsara Driver
properties_list:
- description: Unique Samsara-assigned identifier for the driver.
  name: id
  type: string
- description: Full name of the driver.
  name: name
  type: string
- description: Driver's login username for the Samsara Driver App.
  name: username
  type: string
- description: Whether the driver is active or deactivated.
  name: driverActivationStatus
  type: string
- description: Driver's phone number.
  name: phone
  type: string
- description: Commercial Driver's License (CDL) number.
  name: licenseNumber
  type: string
- description: US state that issued the driver's license (two-letter code).
  name: licenseState
  type: string
- description: ELD/HOS configuration for this driver.
  name: eldSettings
  type: object
- description: Customer-defined key-value pairs for external system identifiers.
  name: externalIds
  type: object
- description: Tags assigned to this driver for organizational grouping.
  name: tags
  type: array
- description: Driver's home timezone (IANA timezone database name, e.g., America/Chicago).
  name: timezone
  type: string
- description: The vehicle currently assigned to this driver.
  name: currentVehicle
  type: object
provider_name: Samsara
provider_slug: samsara
schema_file: json-schema/samsara-driver-schema.json
slug: samsara-driver
source_filename: samsara-driver-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"samsara-driver-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Samsara Driver\",\n  \"description\": \"Schema for a Samsara driver entity as returned by the Samsara REST API. Represents a commercial vehicle driver managed in the Samsara platform.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Samsara-assigned identifier for the driver.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the driver.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Driver's login username for the Samsara Driver App.\"\n    },\n    \"driverActivationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Whether the driver is active or deactivated.\",\n      \"enum\": [\"active\", \"deactivated\"]\n    },\n    \"phone\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"Driver's phone number.\"\n    },\n    \"licenseNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Commercial Driver's License (CDL) number.\"\n    },\n    \"licenseState\": {\n      \"type\": \"string\",\n      \"description\": \"US state that issued the driver's license (two-letter code).\",\n      \"pattern\": \"^[A-Z]{2}$\"\n    },\n    \"eldSettings\": {\n      \"type\": \"object\",\n      \"description\": \"ELD/HOS configuration for this driver.\",\n      \"properties\": {\n        \"eldAdverseWeatherExemptionEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the adverse weather HOS exemption is enabled.\"\n        },\n        \"eldBigDayExemptionEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the big day HOS exemption is enabled.\"\n        },\n        \"eldDayStartHour\": {\n          \"type\": \"integer\",\n          \"description\": \"The\
  \ hour of the day at which HOS rollover occurs (0-23).\",\n          \"minimum\": 0,\n          \"maximum\": 23\n        },\n        \"eldExempt\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this driver is ELD-exempt.\"\n        },\n        \"eldExemptReason\": {\n          \"type\": \"string\",\n          \"description\": \"Reason for ELD exemption.\"\n        },\n        \"eldPcEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether personal conveyance (PC) is enabled.\"\n        },\n        \"eldYmEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether yard moves (YM) are enabled.\"\n        },\n        \"rulesets\": {\n          \"type\": \"array\",\n          \"description\": \"HOS rulesets applicable to this driver.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"cycle\": {\n                \"type\": \"string\",\n                \"\
  description\": \"HOS cycle (e.g., USA Property 70hr/8days, Canada 70hr/7days).\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"externalIds\": {\n      \"type\": \"object\",\n      \"description\": \"Customer-defined key-value pairs for external system identifiers.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags assigned to this driver for organizational grouping.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Driver's home timezone (IANA timezone database name, e.g., America/Chicago).\"\n    },\n    \"currentVehicle\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"The vehicle currently assigned to this driver.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/samsara/refs/heads/main/json-schema/samsara-driver-schema.json
tags:
- Asset Tracking
- Connected Operations
- ELD
- Fleet Management
- GPS Tracking
- IoT
- Logistics
- Safety
- Telematics
- Transportation
title: Samsara Driver
---
