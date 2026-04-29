---
description: UninstallAndroidCertificateDetails schema from Adyen API
layout: schema
name: UninstallAndroidCertificateDetails
properties_list:
- description: The unique identifier of the certificate to be uninstalled.
  name: certificateId
  type: string
- description: 'Type of terminal action: Uninstall an Android certificate.'
  name: type
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-uninstall-android-certificate-details-schema.json
slug: management-uninstall-android-certificate-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-uninstall-android-certificate-details-schema.json\",\n  \"title\": \"UninstallAndroidCertificateDetails\",\n  \"description\": \"UninstallAndroidCertificateDetails schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"certificateId\": {\n      \"description\": \"The unique identifier of the certificate to be uninstalled.\",\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"default\": \"UninstallAndroidCertificate\",\n      \"description\": \"Type of terminal action: Uninstall an Android certificate.\",\n      \"enum\": [\n        \"UninstallAndroidCertificate\"\n      ],\n      \"type\": \"string\"\n    }\n  },\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-uninstall-android-certificate-details-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: UninstallAndroidCertificateDetails
---
