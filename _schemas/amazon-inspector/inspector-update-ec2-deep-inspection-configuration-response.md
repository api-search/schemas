---
description: UpdateEc2DeepInspectionConfigurationResponse schema
layout: schema
name: UpdateEc2DeepInspectionConfigurationResponse
properties_list:
- description: ''
  name: errorMessage
  type: object
- description: ''
  name: orgPackagePaths
  type: object
- description: ''
  name: packagePaths
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-update-ec2-deep-inspection-configuration-response-schema.json
slug: inspector-update-ec2-deep-inspection-configuration-response
source_filename: inspector-update-ec2-deep-inspection-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-update-ec2-deep-inspection-configuration-response-schema.json\",\n  \"title\": \"UpdateEc2DeepInspectionConfigurationResponse\",\n  \"description\": \"UpdateEc2DeepInspectionConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"An error message explaining why new Amazon Inspector deep inspection custom paths could not be added.\"\n        }\n      ]\n    },\n    \"orgPackagePaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathList\"\n        },\n        {\n          \"description\": \"The current Amazon Inspector deep inspection custom paths for the organization.\"\
  \n        }\n      ]\n    },\n    \"packagePaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathList\"\n        },\n        {\n          \"description\": \"The current Amazon Inspector deep inspection custom paths for your account.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2DeepInspectionStatus\"\n        },\n        {\n          \"description\": \"The status of Amazon Inspector deep inspection in your account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-update-ec2-deep-inspection-configuration-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: UpdateEc2DeepInspectionConfigurationResponse
---
