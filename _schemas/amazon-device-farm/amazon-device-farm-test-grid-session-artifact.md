---
description: Artifacts are video and other files that are produced in the process of running a browser in an automated context. Video elements might be broken up into multiple artifacts as they grow in size during creation.
layout: schema
name: TestGridSessionArtifact
properties_list:
- description: ''
  name: filename
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: url
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-test-grid-session-artifact-schema.json
slug: amazon-device-farm-test-grid-session-artifact
source_filename: amazon-device-farm-test-grid-session-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-session-artifact-schema.json\",\n  \"title\": \"TestGridSessionArtifact\",\n  \"description\": \"Artifacts are video and other files that are produced in the process of running a browser in an automated context.   Video elements might be broken up into multiple artifacts as they grow in size during creation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filename\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The file name of the artifact.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TestGridSessionArtifactType\"\n        },\n        {\n          \"description\": \"The kind of artifact.\"\n  \
  \      }\n      ]\n    },\n    \"url\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveString\"\n        },\n        {\n          \"description\": \"A semi-stable URL to the content of the object.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-test-grid-session-artifact-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: TestGridSessionArtifact
---
