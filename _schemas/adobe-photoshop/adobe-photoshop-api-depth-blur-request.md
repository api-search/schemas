---
description: DepthBlurRequest from Adobe Photoshop API
layout: schema
name: DepthBlurRequest
properties_list:
- description: ''
  name: inputs
  type: array
- description: ''
  name: options
  type: object
- description: ''
  name: outputs
  type: array
provider_name: Adobe Photoshop
provider_slug: adobe-photoshop
schema_file: json-schema/adobe-photoshop-api-depth-blur-request-schema.json
slug: adobe-photoshop-api-depth-blur-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-depth-blur-request-schema.json\",\n  \"title\": \"DepthBlurRequest\",\n  \"description\": \"DepthBlurRequest from Adobe Photoshop API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageInput\"\n      }\n    },\n    \"options\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"focalSelector\": {\n          \"type\": \"object\",\n          \"description\": \"Coordinates of the focal point.\"\n        },\n        \"focalDistance\": {\n          \"type\": \"number\",\n          \"description\": \"Distance to the focal point.\"\n        },\n        \"blurStrength\": {\n          \"type\": \"number\",\n          \"description\": \"Intensity of the blur effect.\"\
  \n        },\n        \"focalRange\": {\n          \"type\": \"number\",\n          \"description\": \"Range of the focal area.\"\n        },\n        \"grain\": {\n          \"type\": \"number\",\n          \"description\": \"Amount of film grain to add.\"\n        },\n        \"haze\": {\n          \"type\": \"number\",\n          \"description\": \"Amount of atmospheric haze to add.\"\n        }\n      }\n    },\n    \"outputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/StorageOutput\"\n      }\n    }\n  },\n  \"required\": [\n    \"inputs\",\n    \"outputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-photoshop/refs/heads/main/json-schema/adobe-photoshop-api-depth-blur-request-schema.json
tags:
- AI/ML
- Creative Cloud
- Image Editing
- Photoshop
- Plugins
- REST API
- Scripting
title: DepthBlurRequest
---
