---
description: Esam
layout: schema
name: Esam
properties_list:
- description: ''
  name: AcquisitionPointId
  type: object
- description: ''
  name: AdAvailOffset
  type: object
- description: ''
  name: PasswordParam
  type: object
- description: ''
  name: PoisEndpoint
  type: object
- description: ''
  name: Username
  type: object
- description: ''
  name: ZoneIdentity
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-esam-schema.json
slug: medialive-api-esam
source_filename: medialive-api-esam-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-esam-schema.json\",\n  \"title\": \"Esam\",\n  \"description\": \"Esam\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AcquisitionPointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"acquisitionPointId\"\n          },\n          \"description\": \"Sent as acquisitionPointIdentity to identify the MediaLive channel to the POIS.\"\n        }\n      ]\n    },\n    \"AdAvailOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative1000Max1000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"adAvailOffset\"\n          },\n          \"description\": \"When specified, this offset (in milliseconds)\
  \ is added to the input Ad Avail PTS time. This only applies to embedded SCTE 104/35 messages and does not apply to OOB messages.\"\n        }\n      ]\n    },\n    \"PasswordParam\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"passwordParam\"\n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    },\n    \"PoisEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax2048\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"poisEndpoint\"\n          },\n          \"description\": \"The URL of the signal conditioner endpoint on the Placement Opportunity Information System (POIS). MediaLive sends SignalProcessingEvents here when SCTE-35 messages are read.\"\n        }\n      ]\n    },\n    \"Username\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"username\"\n          },\n          \"description\": \"Documentation update needed\"\n        }\n      ]\n    },\n    \"ZoneIdentity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMax256\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"zoneIdentity\"\n          },\n          \"description\": \"Optional data sent as zoneIdentity to identify the MediaLive channel to the POIS.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AcquisitionPointId\",\n    \"PoisEndpoint\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-esam-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Esam
---
