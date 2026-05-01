---
description: DescribeClientBrandingResult schema from Amazon WorkSpaces API
layout: schema
name: DescribeClientBrandingResult
properties_list:
- description: ''
  name: DeviceTypeWindows
  type: object
- description: ''
  name: DeviceTypeOsx
  type: object
- description: ''
  name: DeviceTypeAndroid
  type: object
- description: ''
  name: DeviceTypeIos
  type: object
- description: ''
  name: DeviceTypeLinux
  type: object
- description: ''
  name: DeviceTypeWeb
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-describe-client-branding-result-schema.json
slug: workspaces-describe-client-branding-result
source_filename: workspaces-describe-client-branding-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeviceTypeWindows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information for Windows devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeOsx\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information for macOS devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeAndroid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information for Android devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeIos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IosClientBrandingAttributes\"\n        },\n\
  \        {\n          \"description\": \"The branding information for iOS devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeLinux\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information for Linux devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeWeb\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information for Web access.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeClientBrandingResult\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-branding-result-schema.json\",\n  \"description\": \"DescribeClientBrandingResult schema from Amazon WorkSpaces\
  \ API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-describe-client-branding-result-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: DescribeClientBrandingResult
---
