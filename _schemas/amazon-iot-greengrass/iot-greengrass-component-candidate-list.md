---
description: ComponentCandidateList schema
layout: schema
name: ComponentCandidateList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-candidate-list-schema.json
slug: iot-greengrass-component-candidate-list
source_filename: iot-greengrass-component-candidate-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-candidate-list-schema.json\",\n  \"title\": \"ComponentCandidateList\",\n  \"description\": \"ComponentCandidateList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"componentName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentNameString\"\n          },\n          {\n            \"description\": \"The name of the component.\"\n          }\n        ]\n      },\n      \"componentVersion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentVersionString\"\n          },\n          {\n            \"description\": \"The version of the component.\"\n          }\n        ]\n      },\n      \"versionRequirements\": {\n        \"allOf\"\
  : [\n          {\n            \"$ref\": \"#/components/schemas/ComponentVersionRequirementMap\"\n          },\n          {\n            \"description\": \"<p>The version requirements for the component's dependencies. Greengrass core devices get the version requirements from component recipes.</p> <p>IoT Greengrass V2 uses semantic version constraints. For more information, see <a href=\\\"https://semver.org/\\\">Semantic Versioning</a>.</p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a component that is a candidate to deploy to a Greengrass core device.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-candidate-list-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentCandidateList
---
