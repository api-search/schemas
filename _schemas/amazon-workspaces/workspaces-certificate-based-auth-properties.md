---
description: Describes the properties of the certificate-based authentication you want to use with your WorkSpaces.
layout: schema
name: CertificateBasedAuthProperties
properties_list:
- description: ''
  name: Status
  type: object
- description: ''
  name: CertificateAuthorityArn
  type: object
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
schema_file: json-schema/workspaces-certificate-based-auth-properties-schema.json
slug: workspaces-certificate-based-auth-properties
source_filename: workspaces-certificate-based-auth-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateBasedAuthStatusEnum\"\n        },\n        {\n          \"description\": \"The status of the certificate-based authentication properties.\"\n        }\n      ]\n    },\n    \"CertificateAuthorityArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Amazon Web Services Certificate Manager Private CA resource.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Describes the properties of the certificate-based authentication you want to use with your WorkSpaces.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateBasedAuthProperties\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-certificate-based-auth-properties-schema.json\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces/refs/heads/main/json-schema/workspaces-certificate-based-auth-properties-schema.json
tags:
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
title: CertificateBasedAuthProperties
---
