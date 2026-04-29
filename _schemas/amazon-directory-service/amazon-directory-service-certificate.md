---
description: Information about the certificate.
layout: schema
name: Certificate
properties_list:
- description: ''
  name: CertificateId
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: StateReason
  type: object
- description: ''
  name: CommonName
  type: object
- description: ''
  name: RegisteredDateTime
  type: object
- description: ''
  name: ExpiryDateTime
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: ClientCertAuthSettings
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-certificate-schema.json
slug: amazon-directory-service-certificate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-certificate-schema.json\",\n  \"title\": \"Certificate\",\n  \"description\": \"Information about the certificate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateId\"\n        },\n        {\n          \"description\": \"The identifier of the certificate.\"\n        }\n      ]\n    },\n    \"State\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateState\"\n        },\n        {\n          \"description\": \"The state of the certificate.\"\n        }\n      ]\n    },\n    \"StateReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateStateReason\"\n        },\n        {\n      \
  \    \"description\": \"Describes a state change for the certificate.\"\n        }\n      ]\n    },\n    \"CommonName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateCN\"\n        },\n        {\n          \"description\": \"The common name for the certificate.\"\n        }\n      ]\n    },\n    \"RegisteredDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateRegisteredDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the certificate was registered.\"\n        }\n      ]\n    },\n    \"ExpiryDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateExpiryDateTime\"\n        },\n        {\n          \"description\": \"The date and time when the certificate will expire.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CertificateType\"\n        },\n \
  \       {\n          \"description\": \"The function that the registered certificate performs. Valid values include <code>ClientLDAPS</code> or <code>ClientCertAuth</code>. The default value is <code>ClientLDAPS</code>.\"\n        }\n      ]\n    },\n    \"ClientCertAuthSettings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientCertAuthSettings\"\n        },\n        {\n          \"description\": \"A <code>ClientCertAuthSettings</code> object that contains client certificate authentication settings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-certificate-schema.json
tags:
- Active Directory
- Authentication
- AWS
- Directory Services
- Identity Management
title: Certificate
---
