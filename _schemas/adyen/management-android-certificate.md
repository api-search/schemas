---
description: AndroidCertificate schema from Adyen API
layout: schema
name: AndroidCertificate
properties_list:
- description: The description that was provided when uploading the certificate.
  name: description
  type: string
- description: The file format of the certificate, as indicated by the file extension. For example, **.cert** or **.pem**.
  name: extension
  type: string
- description: The unique identifier of the certificate.
  name: id
  type: string
- description: The file name of the certificate. For example, **mycert**.
  name: name
  type: string
- description: The date when the certificate stops to be valid.
  name: notAfter
  type: string
- description: The date when the certificate starts to be valid.
  name: notBefore
  type: string
- description: The status of the certificate.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-android-certificate-schema.json
slug: management-android-certificate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-android-certificate-schema.json\",\n  \"title\": \"AndroidCertificate\",\n  \"description\": \"AndroidCertificate schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"The description that was provided when uploading the certificate.\",\n      \"type\": \"string\"\n    },\n    \"extension\": {\n      \"description\": \"The file format of the certificate, as indicated by the file extension. For example, **.cert** or **.pem**.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the certificate.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The file name of the certificate. For example, **mycert**.\",\n      \"type\": \"string\"\n    },\n    \"notAfter\"\
  : {\n      \"description\": \"The date when the certificate stops to be valid.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"notBefore\": {\n      \"description\": \"The date when the certificate starts to be valid.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the certificate.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-android-certificate-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: AndroidCertificate
---
