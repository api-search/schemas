---
description: ComponentDependencyMap schema
layout: schema
name: ComponentDependencyMap
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-dependency-map-schema.json
slug: iot-greengrass-component-dependency-map
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-dependency-map-schema.json\",\n  \"title\": \"ComponentDependencyMap\",\n  \"description\": \"ComponentDependencyMap schema\",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"versionRequirement\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"<p>The component version requirement for the component dependency.</p> <p>IoT Greengrass V2 uses semantic version constraints. For more information, see <a href=\\\"https://semver.org/\\\">Semantic Versioning</a>.</p>\"\n          }\n        ]\n      },\n      \"dependencyType\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentDependencyType\"\
  \n          },\n          {\n            \"description\": \"<p>The type of this dependency. Choose from the following options:</p> <ul> <li> <p> <code>SOFT</code> \\u2013 The component doesn't restart if the dependency changes state.</p> </li> <li> <p> <code>HARD</code> \\u2013 The component restarts if the dependency changes state.</p> </li> </ul> <p>Default: <code>HARD</code> </p>\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a component dependency for a Lambda function component.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-dependency-map-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentDependencyMap
---
