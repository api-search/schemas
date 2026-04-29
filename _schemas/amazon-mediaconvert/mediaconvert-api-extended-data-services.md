---
description: If your source content has EIA-608 Line 21 Data Services, enable this feature to specify what MediaConvert does with the Extended Data Services (XDS) packets. You can choose to pass through XDS packets, or remove them from the output. For more information about XDS, see EIA-608 Line Data Services, section 9.5.1.5 05h Content Advisory.
layout: schema
name: ExtendedDataServices
properties_list:
- description: ''
  name: CopyProtectionAction
  type: object
- description: ''
  name: VchipAction
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-extended-data-services-schema.json
slug: mediaconvert-api-extended-data-services
source_filename: mediaconvert-api-extended-data-services-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-extended-data-services-schema.json\",\n  \"title\": \"ExtendedDataServices\",\n  \"description\": \"If your source content has EIA-608 Line 21 Data Services, enable this feature to specify what MediaConvert does with the Extended Data Services (XDS) packets. You can choose to pass through XDS packets, or remove them from the output. For more information about XDS, see EIA-608 Line Data Services, section 9.5.1.5 05h Content Advisory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CopyProtectionAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CopyProtectionAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"copyProtectionAction\"\n          },\n          \"description\": \"The action to take on copy and redistribution\
  \ control XDS packets. If you select PASSTHROUGH, packets will not be changed. If you select STRIP, any packets will be removed in output captions.\"\n        }\n      ]\n    },\n    \"VchipAction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VchipAction\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"vchipAction\"\n          },\n          \"description\": \"The action to take on content advisory XDS packets. If you select PASSTHROUGH, packets will not be changed. If you select STRIP, any packets will be removed in output captions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-extended-data-services-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ExtendedDataServices
---
