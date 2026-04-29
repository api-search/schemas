---
description: GetEc2DeepInspectionConfigurationResponse schema
layout: schema
name: GetEc2DeepInspectionConfigurationResponse
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
schema_file: json-schema/inspector-get-ec2-deep-inspection-configuration-response-schema.json
slug: inspector-get-ec2-deep-inspection-configuration-response
source_filename: inspector-get-ec2-deep-inspection-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-ec2-deep-inspection-configuration-response-schema.json\",\n  \"title\": \"GetEc2DeepInspectionConfigurationResponse\",\n  \"description\": \"GetEc2DeepInspectionConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"An error message explaining why Amazon Inspector deep inspection configurations could not be retrieved for your account.\"\n        }\n      ]\n    },\n    \"orgPackagePaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathList\"\n        },\n        {\n          \"description\": \"The Amazon Inspector deep inspection custom paths for your organization.\"\
  \n        }\n      ]\n    },\n    \"packagePaths\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PathList\"\n        },\n        {\n          \"description\": \"The Amazon Inspector deep inspection custom paths for your account.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Ec2DeepInspectionStatus\"\n        },\n        {\n          \"description\": \"The activation status of Amazon Inspector deep inspection in your account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-get-ec2-deep-inspection-configuration-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: GetEc2DeepInspectionConfigurationResponse
---
