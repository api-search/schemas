---
description: ModifyCertificateBasedAuthPropertiesRequest schema from Amazon WorkSpaces API
layout: schema
name: ModifyCertificateBasedAuthPropertiesRequest
properties_list:
- description: ''
  name: ResourceId
  type: object
- description: ''
  name: CertificateBasedAuthProperties
  type: object
- description: ''
  name: PropertiesToDelete
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-modify-certificate-based-auth-properties-request-schema.json
slug: workspaces-modify-certificate-based-auth-properties-request
source_filename: workspaces-modify-certificate-based-auth-properties-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"ResourceId\"\n  ],\n  \"title\": \"ModifyCertificateBasedAuthPropertiesRequest\",\n  \"properties\": {\n    \"ResourceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The resource identifiers, in the form of directory IDs.\"\n        }\n      ]\n    },\n    \"CertificateBasedAuthProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateBasedAuthProperties\"\n        },\n        {\n          \"description\": \"The properties of the certificate-based authentication.\"\n        }\n      ]\n    },\n    \"PropertiesToDelete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeletableCertificateBasedAuthPropertiesList\"\n        },\n        {\n          \"description\": \"The properties of the certificate-based authentication you want to delete.\"\n       \
  \ }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-certificate-based-auth-properties-request-schema.json\",\n  \"description\": \"ModifyCertificateBasedAuthPropertiesRequest schema from Amazon WorkSpaces API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-modify-certificate-based-auth-properties-request-schema.json
tags:
- AWS
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: ModifyCertificateBasedAuthPropertiesRequest
---
