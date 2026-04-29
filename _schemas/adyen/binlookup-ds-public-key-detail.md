---
description: DSPublicKeyDetail schema from Adyen API
layout: schema
name: DSPublicKeyDetail
properties_list:
- description: Card brand.
  name: brand
  type: string
- description: Directory Server (DS) identifier.
  name: directoryServerId
  type: string
- description: The version of the mobile 3D Secure 2 SDK. For the possible values, refer to the versions in [Adyen 3DS2 Android](https://github.com/Adyen/adyen-3ds2-android/releases) and [Adyen 3DS2 iOS](https://git
  name: fromSDKVersion
  type: string
- description: Public key. The 3D Secure 2 SDK encrypts the device information by using the DS public key.
  name: publicKey
  type: string
- description: Directory Server root certificates. The 3D Secure 2 SDK verifies the ACS signed content using the rootCertificates.
  name: rootCertificates
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/binlookup-ds-public-key-detail-schema.json
slug: binlookup-ds-public-key-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-ds-public-key-detail-schema.json\",\n  \"title\": \"DSPublicKeyDetail\",\n  \"description\": \"DSPublicKeyDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"description\": \"Card brand.\",\n      \"type\": \"string\"\n    },\n    \"directoryServerId\": {\n      \"description\": \"Directory Server (DS) identifier.\",\n      \"type\": \"string\"\n    },\n    \"fromSDKVersion\": {\n      \"description\": \"The version of the mobile 3D Secure 2 SDK. For the possible values, refer to the versions in [Adyen 3DS2 Android](https://github.com/Adyen/adyen-3ds2-android/releases) and [Adyen 3DS2 iOS](https://github.com/Adyen/adyen-3ds2-ios/releases).\",\n      \"type\": \"string\"\n    },\n    \"publicKey\": {\n      \"description\": \"Public key. The 3D Secure\
  \ 2 SDK encrypts the device information by using the DS public key.\",\n      \"format\": \"byte\",\n      \"type\": \"string\"\n    },\n    \"rootCertificates\": {\n      \"description\": \"Directory Server root certificates. The 3D Secure 2 SDK verifies the ACS signed content using the rootCertificates.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/binlookup-ds-public-key-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: DSPublicKeyDetail
---
