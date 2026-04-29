---
description: GetTrustStoreCertificateResponse schema from Amazon WorkSpaces Web API
layout: schema
name: GetTrustStoreCertificateResponse
properties_list:
- description: ''
  name: certificate
  type: object
- description: ''
  name: trustStoreArn
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-get-trust-store-certificate-response-schema.json
slug: workspaces-web-get-trust-store-certificate-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Certificate\"\n        },\n        {\n          \"description\": \"The certificate of the trust store certificate.\"\n        }\n      ]\n    },\n    \"trustStoreArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN of the trust store certificate.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetTrustStoreCertificateResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-trust-store-certificate-response-schema.json\",\n  \"description\": \"GetTrustStoreCertificateResponse schema from Amazon WorkSpaces Web API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-get-trust-store-certificate-response-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: GetTrustStoreCertificateResponse
---
