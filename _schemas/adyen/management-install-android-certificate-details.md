---
description: InstallAndroidCertificateDetails schema from Adyen API
layout: schema
name: InstallAndroidCertificateDetails
properties_list:
- description: The unique identifier of the certificate to be installed.
  name: certificateId
  type: string
- description: 'Type of terminal action: Install an Android certificate.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-install-android-certificate-details-schema.json
slug: management-install-android-certificate-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-install-android-certificate-details-schema.json\",\n  \"title\": \"InstallAndroidCertificateDetails\",\n  \"description\": \"InstallAndroidCertificateDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateId\": {\n      \"description\": \"The unique identifier of the certificate to be installed.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"InstallAndroidCertificate\",\n      \"description\": \"Type of terminal action: Install an Android certificate.\",\n      \"enum\": [\n        \"InstallAndroidCertificate\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-install-android-certificate-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: InstallAndroidCertificateDetails
---
