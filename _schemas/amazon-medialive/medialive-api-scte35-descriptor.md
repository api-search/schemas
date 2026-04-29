---
description: Holds one set of SCTE-35 Descriptor Settings.
layout: schema
name: Scte35Descriptor
properties_list:
- description: ''
  name: Scte35DescriptorSettings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-scte35-descriptor-schema.json
slug: medialive-api-scte35-descriptor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-descriptor-schema.json\",\n  \"title\": \"Scte35Descriptor\",\n  \"description\": \"Holds one set of SCTE-35 Descriptor Settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Scte35DescriptorSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Scte35DescriptorSettings\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scte35DescriptorSettings\"\n          },\n          \"description\": \"SCTE-35 Descriptor Settings.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Scte35DescriptorSettings\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-scte35-descriptor-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: Scte35Descriptor
---
