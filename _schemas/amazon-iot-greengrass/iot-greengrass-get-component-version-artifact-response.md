---
description: GetComponentVersionArtifactResponse schema
layout: schema
name: GetComponentVersionArtifactResponse
properties_list:
- description: ''
  name: preSignedUrl
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-get-component-version-artifact-response-schema.json
slug: iot-greengrass-get-component-version-artifact-response
source_filename: iot-greengrass-get-component-version-artifact-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-component-version-artifact-response-schema.json\",\n  \"title\": \"GetComponentVersionArtifactResponse\",\n  \"description\": \"GetComponentVersionArtifactResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"preSignedUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The URL of the artifact.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"preSignedUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-component-version-artifact-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: GetComponentVersionArtifactResponse
---
