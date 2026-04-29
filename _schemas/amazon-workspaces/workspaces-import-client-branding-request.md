---
description: ImportClientBrandingRequest schema from Amazon WorkSpaces API
layout: schema
name: ImportClientBrandingRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
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
schema_file: json-schema/workspaces-import-client-branding-request-schema.json
slug: workspaces-import-client-branding-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\"\n  ],\n  \"title\": \"ImportClientBrandingRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The directory identifier of the WorkSpace for which you want to import client branding.\"\n        }\n      ]\n    },\n    \"DeviceTypeWindows\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultImportClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information to import for Windows devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeOsx\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultImportClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information to import for macOS devices.\"\n        }\n      ]\n    },\n \
  \   \"DeviceTypeAndroid\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultImportClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information to import for Android devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeIos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IosImportClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information to import for iOS devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeLinux\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultImportClientBrandingAttributes\"\n        },\n        {\n          \"description\": \"The branding information to import for Linux devices.\"\n        }\n      ]\n    },\n    \"DeviceTypeWeb\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DefaultImportClientBrandingAttributes\"\n        },\n        {\n\
  \          \"description\": \"The branding information to import for web access.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-import-client-branding-request-schema.json\",\n  \"description\": \"ImportClientBrandingRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-import-client-branding-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ImportClientBrandingRequest
---
