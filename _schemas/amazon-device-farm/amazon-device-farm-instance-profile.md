---
description: Represents the instance profile.
layout: schema
name: InstanceProfile
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: packageCleanup
  type: object
- description: ''
  name: excludeAppPackagesFromCleanup
  type: object
- description: ''
  name: rebootAfterUse
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
provider_name: Amazon Device Farm
provider_slug: amazon-device-farm
schema_file: json-schema/amazon-device-farm-instance-profile-schema.json
slug: amazon-device-farm-instance-profile
source_filename: amazon-device-farm-instance-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-instance-profile-schema.json\",\n  \"title\": \"InstanceProfile\",\n  \"description\": \"Represents the instance profile.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the instance profile.\"\n        }\n      ]\n    },\n    \"packageCleanup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"When set to <code>true</code>, Device Farm removes app packages after a test run. The default value is <code>false</code> for private devices.\"\n        }\n      ]\n    },\n    \"excludeAppPackagesFromCleanup\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageIds\"\n        },\n        {\n          \"description\": \"<p>An array of strings containing the list of app packages that should not be cleaned up from the device after a test run completes.</p> <p>The list of packages is considered only if you set <code>packageCleanup</code> to <code>true</code>.</p>\"\n        }\n      ]\n    },\n    \"rebootAfterUse\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"When set to <code>true</code>, Device Farm reboots the instance after a test run. The default value is <code>true</code>.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the instance profile.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/Message\"\n        },\n        {\n          \"description\": \"The description of the instance profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-device-farm/refs/heads/main/json-schema/amazon-device-farm-instance-profile-schema.json
tags:
- Application Testing
- AWS
- Device Testing
- Mobile Testing
- Quality Assurance
title: InstanceProfile
---
