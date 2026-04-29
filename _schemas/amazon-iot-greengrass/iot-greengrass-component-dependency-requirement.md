---
description: Contains information about a component dependency for a Lambda function component.
layout: schema
name: ComponentDependencyRequirement
properties_list:
- description: ''
  name: versionRequirement
  type: object
- description: ''
  name: dependencyType
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-dependency-requirement-schema.json
slug: iot-greengrass-component-dependency-requirement
source_filename: iot-greengrass-component-dependency-requirement-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-dependency-requirement-schema.json\",\n  \"title\": \"ComponentDependencyRequirement\",\n  \"description\": \"Contains information about a component dependency for a Lambda function component.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versionRequirement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The component version requirement for the component dependency.</p> <p>IoT Greengrass V2 uses semantic version constraints. For more information, see <a href=\\\"https://semver.org/\\\">Semantic Versioning</a>.</p>\"\n        }\n      ]\n    },\n    \"dependencyType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentDependencyType\"\
  \n        },\n        {\n          \"description\": \"<p>The type of this dependency. Choose from the following options:</p> <ul> <li> <p> <code>SOFT</code> \\u2013 The component doesn't restart if the dependency changes state.</p> </li> <li> <p> <code>HARD</code> \\u2013 The component restarts if the dependency changes state.</p> </li> </ul> <p>Default: <code>HARD</code> </p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-dependency-requirement-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentDependencyRequirement
---
