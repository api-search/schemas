---
description: Settings for Event Signaling And Messaging (ESAM). If you don't do ad insertion, you can ignore these settings.
layout: schema
name: EsamSettings
properties_list:
- description: ''
  name: ManifestConfirmConditionNotification
  type: object
- description: ''
  name: ResponseSignalPreroll
  type: object
- description: ''
  name: SignalProcessingNotification
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-esam-settings-schema.json
slug: mediaconvert-api-esam-settings
source_filename: mediaconvert-api-esam-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-esam-settings-schema.json\",\n  \"title\": \"EsamSettings\",\n  \"description\": \"Settings for Event Signaling And Messaging (ESAM). If you don't do ad insertion, you can ignore these settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManifestConfirmConditionNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EsamManifestConfirmConditionNotification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestConfirmConditionNotification\"\n          },\n          \"description\": \"Specifies an ESAM ManifestConfirmConditionNotification XML as per OC-SP-ESAM-API-I03-131025. The transcoder uses the manifest conditioning instructions that you provide in the setting MCC XML (mccXml).\"\n        }\n      ]\n  \
  \  },\n    \"ResponseSignalPreroll\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max30000\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"responseSignalPreroll\"\n          },\n          \"description\": \"Specifies the stream distance, in milliseconds, between the SCTE 35 messages that the transcoder places and the splice points that they refer to. If the time between the start of the asset and the SCTE-35 message is less than this value, then the transcoder places the SCTE-35 marker at the beginning of the stream.\"\n        }\n      ]\n    },\n    \"SignalProcessingNotification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EsamSignalProcessingNotification\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"signalProcessingNotification\"\n          },\n          \"description\": \"Specifies an ESAM SignalProcessingNotification XML as per OC-SP-ESAM-API-I03-131025.\
  \ The transcoder uses the signal processing instructions that you provide in the setting SCC XML (sccXml).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-esam-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EsamSettings
---
