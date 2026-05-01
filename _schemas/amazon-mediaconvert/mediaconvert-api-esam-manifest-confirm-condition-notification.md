---
description: ESAM ManifestConfirmConditionNotification defined by OC-SP-ESAM-API-I03-131025.
layout: schema
name: EsamManifestConfirmConditionNotification
properties_list:
- description: ''
  name: MccXml
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-esam-manifest-confirm-condition-notification-schema.json
slug: mediaconvert-api-esam-manifest-confirm-condition-notification
source_filename: mediaconvert-api-esam-manifest-confirm-condition-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-esam-manifest-confirm-condition-notification-schema.json\",\n  \"title\": \"EsamManifestConfirmConditionNotification\",\n  \"description\": \"ESAM ManifestConfirmConditionNotification defined by OC-SP-ESAM-API-I03-131025.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MccXml\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringPatternSNManifestConfirmConditionNotificationNS\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mccXml\"\n          },\n          \"description\": \"Provide your ESAM ManifestConfirmConditionNotification XML document inside your JSON job settings. Form the XML document as per OC-SP-ESAM-API-I03-131025. The transcoder will use the Manifest Conditioning instructions in the message that you supply.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-esam-manifest-confirm-condition-notification-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: EsamManifestConfirmConditionNotification
---
