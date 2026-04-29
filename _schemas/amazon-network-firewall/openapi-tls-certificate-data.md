---
description: Contains metadata about an Certificate Manager certificate.
layout: schema
name: TlsCertificateData
properties_list:
- description: ''
  name: CertificateArn
  type: object
- description: ''
  name: CertificateSerial
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusMessage
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-tls-certificate-data-schema.json
slug: openapi-tls-certificate-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tls-certificate-data-schema.json\",\n  \"title\": \"TlsCertificateData\",\n  \"description\": \"Contains metadata about an Certificate Manager certificate.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the certificate.\"\n        }\n      ]\n    },\n    \"CertificateSerial\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CollectionMember_String\"\n        },\n        {\n          \"description\": \"The serial number of the certificate.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CollectionMember_String\"\
  \n        },\n        {\n          \"description\": \"The status of the certificate.\"\n        }\n      ]\n    },\n    \"StatusMessage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatusReason\"\n        },\n        {\n          \"description\": \"Contains details about the certificate status, including information about certificate errors.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-tls-certificate-data-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: TlsCertificateData
---
