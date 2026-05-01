---
description: DescribeApplicationInstanceDetailsResponse schema from Amazon Panorama
layout: schema
name: DescribeApplicationInstanceDetailsResponse
properties_list:
- description: ''
  name: ApplicationInstanceId
  type: object
- description: ''
  name: ApplicationInstanceIdToReplace
  type: object
- description: ''
  name: CreatedTime
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
provider_name: Amazon Panorama
provider_slug: amazon-panorama
schema_file: json-schema/openapi-describe-application-instance-details-response-schema.json
slug: openapi-describe-application-instance-details-response
source_filename: openapi-describe-application-instance-details-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-application-instance-details-response-schema.json\",\n  \"title\": \"DescribeApplicationInstanceDetailsResponse\",\n  \"description\": \"DescribeApplicationInstanceDetailsResponse schema from Amazon Panorama\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationInstanceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"The application instance's ID.\"\n        }\n      ]\n    },\n    \"ApplicationInstanceIdToReplace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceId\"\n        },\n        {\n          \"description\": \"The ID of the application instance that this instance replaced.\"\n        }\n      ]\n    },\n \
  \   \"CreatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeStamp\"\n        },\n        {\n          \"description\": \"When the application instance was created.\"\n        }\n      ]\n    },\n    \"DefaultRuntimeContextDevice\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultRuntimeContextDevice\"\n        },\n        {\n          \"description\": \"The application instance's default runtime context device.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The application instance's description.\"\n        }\n      ]\n    },\n    \"ManifestOverridesPayload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestOverridesPayload\"\n        },\n        {\n          \"description\": \"Parameter overrides for the configuration manifest.\"\
  \n        }\n      ]\n    },\n    \"ManifestPayload\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManifestPayload\"\n        },\n        {\n          \"description\": \"The application instance's configuration manifest.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationInstanceName\"\n        },\n        {\n          \"description\": \"The application instance's name.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-panorama/refs/heads/main/json-schema/openapi-describe-application-instance-details-response-schema.json
tags:
- Cameras
- Computer Vision
- Edge ML
- Industrial IoT
title: DescribeApplicationInstanceDetailsResponse
---
