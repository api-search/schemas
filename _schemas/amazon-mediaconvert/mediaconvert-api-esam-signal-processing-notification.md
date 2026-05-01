---
description: ESAM SignalProcessingNotification data defined by OC-SP-ESAM-API-I03-131025.
layout: schema
name: EsamSignalProcessingNotification
properties_list:
- description: ''
  name: SccXml
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-esam-signal-processing-notification-schema.json
slug: mediaconvert-api-esam-signal-processing-notification
source_filename: mediaconvert-api-esam-signal-processing-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-esam-signal-processing-notification-schema.json\",\n  \"title\": \"EsamSignalProcessingNotification\",\n  \"description\": \"ESAM SignalProcessingNotification data defined by OC-SP-ESAM-API-I03-131025.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SccXml\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternSNSignalProcessingNotificationNS\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sccXml\"\n          },\n          \"description\": \"Provide your ESAM SignalProcessingNotification XML document inside your JSON job settings. Form the XML document as per OC-SP-ESAM-API-I03-131025. The transcoder will use the signal processing instructions in the message that you supply. Provide your ESAM SignalProcessingNotification\
  \ XML document inside your JSON job settings. For your MPEG2-TS file outputs, if you want the service to place SCTE-35 markers at the insertion points you specify in the XML document, you must also enable SCTE-35 ESAM (scte35Esam). Note that you can either specify an ESAM XML document or enable SCTE-35 passthrough. You can't do both.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-esam-signal-processing-notification-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EsamSignalProcessingNotification
---
