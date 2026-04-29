---
description: Corresponds to SCTE-35 delivery_not_restricted_flag parameter. To declare delivery restrictions, include this element and its four "restriction" flags. To declare that there are no restrictions, omit this element.
layout: schema
name: Scte35DeliveryRestrictions
properties_list:
- description: ''
  name: ArchiveAllowedFlag
  type: object
- description: ''
  name: DeviceRestrictions
  type: object
- description: ''
  name: NoRegionalBlackoutFlag
  type: object
- description: ''
  name: WebDeliveryAllowedFlag
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-delivery-restrictions-schema.json
slug: medialive-api-scte35-delivery-restrictions
source_filename: medialive-api-scte35-delivery-restrictions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-delivery-restrictions-schema.json\",\n  \"title\": \"Scte35DeliveryRestrictions\",\n  \"description\": \"Corresponds to SCTE-35 delivery_not_restricted_flag parameter. To declare delivery restrictions, include this element and its four \\\"restriction\\\" flags. To declare that there are no restrictions, omit this element.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArchiveAllowedFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35ArchiveAllowedFlag\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"archiveAllowedFlag\"\n          },\n          \"description\": \"Corresponds to SCTE-35 archive_allowed_flag.\"\n        }\n      ]\n    },\n    \"DeviceRestrictions\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/Scte35DeviceRestrictions\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"deviceRestrictions\"\n          },\n          \"description\": \"Corresponds to SCTE-35 device_restrictions parameter.\"\n        }\n      ]\n    },\n    \"NoRegionalBlackoutFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35NoRegionalBlackoutFlag\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"noRegionalBlackoutFlag\"\n          },\n          \"description\": \"Corresponds to SCTE-35 no_regional_blackout_flag parameter.\"\n        }\n      ]\n    },\n    \"WebDeliveryAllowedFlag\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35WebDeliveryAllowedFlag\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"webDeliveryAllowedFlag\"\n          },\n          \"description\": \"Corresponds to SCTE-35 web_delivery_allowed_flag parameter.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"DeviceRestrictions\",\n    \"ArchiveAllowedFlag\",\n    \"WebDeliveryAllowedFlag\",\n    \"NoRegionalBlackoutFlag\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-delivery-restrictions-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte35DeliveryRestrictions
---
