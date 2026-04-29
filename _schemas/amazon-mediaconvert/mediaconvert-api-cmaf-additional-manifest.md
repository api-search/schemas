---
description: Specify the details for each pair of HLS and DASH additional manifests that you want the service to generate for this CMAF output group. Each pair of manifests can reference a different subset of outputs in the group.
layout: schema
name: CmafAdditionalManifest
properties_list:
- description: ''
  name: ManifestNameModifier
  type: object
- description: ''
  name: SelectedOutputs
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-cmaf-additional-manifest-schema.json
slug: mediaconvert-api-cmaf-additional-manifest
source_filename: mediaconvert-api-cmaf-additional-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-additional-manifest-schema.json\",\n  \"title\": \"CmafAdditionalManifest\",\n  \"description\": \"Specify the details for each pair of HLS and DASH additional manifests that you want the service to generate for this CMAF output group. Each pair of manifests can reference a different subset of outputs in the group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ManifestNameModifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"manifestNameModifier\"\n          },\n          \"description\": \"Specify a name modifier that the service adds to the name of this manifest to make it different from the file names of the other main manifests in the output group.\
  \ For example, say that the default main manifest for your HLS group is film-name.m3u8. If you enter \\\"-no-premium\\\" for this setting, then the file name the service generates for this top-level manifest is film-name-no-premium.m3u8. For HLS output groups, specify a manifestNameModifier that is different from the nameModifier of the output. The service uses the output name modifier to create unique names for the individual variant manifests.\"\n        }\n      ]\n    },\n    \"SelectedOutputs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOf__stringMin1\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"selectedOutputs\"\n          },\n          \"description\": \"Specify the outputs that you want this additional top-level manifest to reference.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-cmaf-additional-manifest-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CmafAdditionalManifest
---
