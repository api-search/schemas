---
description: The certificate issuer indentifier.
layout: schema
name: IssuerCertificateIdentifier
properties_list:
- description: ''
  name: issuerCertificateSubject
  type: object
- description: ''
  name: issuerId
  type: object
- description: ''
  name: issuerCertificateSerialNumber
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-issuer-certificate-identifier-schema.json
slug: iot-device-defender-issuer-certificate-identifier
source_filename: iot-device-defender-issuer-certificate-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-issuer-certificate-identifier-schema.json\",\n  \"title\": \"IssuerCertificateIdentifier\",\n  \"description\": \"The certificate issuer indentifier.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"issuerCertificateSubject\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IssuerCertificateSubject\"\n        },\n        {\n          \"description\": \"The subject of the issuer certificate.\"\n        }\n      ]\n    },\n    \"issuerId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IssuerId\"\n        },\n        {\n          \"description\": \"The issuer ID.\"\n        }\n      ]\n    },\n    \"issuerCertificateSerialNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IssuerCertificateSerialNumber\"\
  \n        },\n        {\n          \"description\": \"The issuer certificate serial number.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-issuer-certificate-identifier-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: IssuerCertificateIdentifier
---
