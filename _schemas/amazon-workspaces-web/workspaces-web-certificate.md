---
description: The certificate.
layout: schema
name: Certificate
properties_list:
- description: ''
  name: body
  type: object
- description: ''
  name: issuer
  type: object
- description: ''
  name: notValidAfter
  type: object
- description: ''
  name: notValidBefore
  type: object
- description: ''
  name: subject
  type: object
- description: ''
  name: thumbprint
  type: object
provider_name: Amazon WorkSpaces Web
provider_slug: amazon-workspaces-web
schema_file: json-schema/workspaces-web-certificate-schema.json
slug: workspaces-web-certificate
source_filename: workspaces-web-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateAuthorityBody\"\n        },\n        {\n          \"description\": \"The body of the certificate.\"\n        }\n      ]\n    },\n    \"issuer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificatePrincipal\"\n        },\n        {\n          \"description\": \"The entity that issued the certificate.\"\n        }\n      ]\n    },\n    \"notValidAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The certificate is not valid after this date.\"\n        }\n      ]\n    },\n    \"notValidBefore\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The certificate is not valid before this date.\"\n        }\n\
  \      ]\n    },\n    \"subject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificatePrincipal\"\n        },\n        {\n          \"description\": \"The entity the certificate belongs to.\"\n        }\n      ]\n    },\n    \"thumbprint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateThumbprint\"\n        },\n        {\n          \"description\": \"A hexadecimal identifier for the certificate.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The certificate.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Certificate\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-certificate-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workspaces-web/refs/heads/main/json-schema/workspaces-web-certificate-schema.json
tags:
- AWS
- End User Computing
- Secure Browser
- Virtual Desktop
- Zero Trust
title: Certificate
---
