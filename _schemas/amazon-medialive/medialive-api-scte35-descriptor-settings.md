---
description: SCTE-35 Descriptor settings.
layout: schema
name: Scte35DescriptorSettings
properties_list:
- description: ''
  name: SegmentationDescriptorScte35DescriptorSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-descriptor-settings-schema.json
slug: medialive-api-scte35-descriptor-settings
source_filename: medialive-api-scte35-descriptor-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-descriptor-settings-schema.json\",\n  \"title\": \"Scte35DescriptorSettings\",\n  \"description\": \"SCTE-35 Descriptor settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SegmentationDescriptorScte35DescriptorSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35SegmentationDescriptor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"segmentationDescriptorScte35DescriptorSettings\"\n          },\n          \"description\": \"SCTE-35 Segmentation Descriptor.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"SegmentationDescriptorScte35DescriptorSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-descriptor-settings-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: Scte35DescriptorSettings
---
