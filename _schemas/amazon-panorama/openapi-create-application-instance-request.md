---
description: CreateApplicationInstanceRequest schema from Amazon Panorama
layout: schema
name: CreateApplicationInstanceRequest
properties_list:
- description: ''
  name: ApplicationInstanceIdToReplace
  type: object
- description: ''
  name: DefaultRuntimeContextDevice
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: ManifestOverridesPayload
  type: object
- description: ''
  name: ManifestPayload
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RuntimeRoleArn
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-create-application-instance-request-schema.json
slug: openapi-create-application-instance-request
source_filename: openapi-create-application-instance-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-application-instance-request-schema.json\",\n  \"title\": \"CreateApplicationInstanceRequest\",\n  \"description\": \"CreateApplicationInstanceRequest schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationInstanceIdToReplace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"The ID of an application instance to replace with the new instance.\"\n        }\n      ]\n    },\n    \"DefaultRuntimeContextDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultRuntimeContextDevice\"\n        },\n        {\n          \"description\": \"A device's ID.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"A description for the application instance.\"\n        }\n      ]\n    },\n    \"ManifestOverridesPayload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestOverridesPayload\"\n        },\n        {\n          \"description\": \"Setting overrides for the application manifest.\"\n        }\n      ]\n    },\n    \"ManifestPayload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestPayload\"\n        },\n        {\n          \"description\": \"The application's manifest document.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceName\"\n        },\n        {\n          \"description\": \"A name for the application instance.\"\n        }\n      ]\n    },\n    \"RuntimeRoleArn\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeRoleArn\"\n        },\n        {\n          \"description\": \"The ARN of a runtime role for the application instance.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"Tags for the application instance.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DefaultRuntimeContextDevice\",\n    \"ManifestPayload\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-create-application-instance-request-schema.json
tags:
- AWS
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: CreateApplicationInstanceRequest
---
