---
description: Profile schema from Adyen API
layout: schema
name: Profile
properties_list:
- description: 'The type of Wi-Fi network. Possible values: **wpa-psk**, **wpa2-psk**, **wpa-eap**, **wpa2-eap**.'
  name: authType
  type: string
- description: Indicates whether to automatically select the best authentication method available. Does not work on older terminal models.
  name: autoWifi
  type: boolean
- description: Use **infra** for infrastructure-based networks. This applies to most networks. Use **adhoc** only if the communication is p2p-based between base stations.
  name: bssType
  type: string
- description: The channel number of the Wi-Fi network. The recommended setting is **0** for automatic channel selection.
  name: channel
  type: integer
- description: Indicates whether this is your preferred wireless network. If **true**, the terminal will try connecting to this network first.
  name: defaultProfile
  type: boolean
- description: 'For `authType` **wpa-eap** or **wpa2-eap**. Possible values: **tls**, **peap**, **leap**, **fast**'
  name: eap
  type: string
- description: For `authType` **wpa-eap** or **wpa2-eap**. The root certificate from the CA that signed the certificate of the RADIUS server that is part of your wireless network.
  name: eapCaCert
  type: object
- description: For `eap` **tls**. The certificate chain for the terminals. All terminals in the same network will use the same EAP client certificate.
  name: eapClientCert
  type: object
- description: For `eap` **tls**. The RSA private key for the client. Include the lines BEGIN RSA PRIVATE KEY and END RSA PRIVATE KEY.
  name: eapClientKey
  type: object
- description: For `eap` **tls**. The password of the RSA key file, if that file is password-protected.
  name: eapClientPwd
  type: string
- description: For `authType` **wpa-eap** or **wpa2-eap**. The EAP-PEAP username from your MS-CHAP account. Must match the configuration of your RADIUS server.
  name: eapIdentity
  type: string
- description: For `eap` **tls**. The EAP intermediate certificate.
  name: eapIntermediateCert
  type: object
- description: For `eap` **peap**. The EAP-PEAP password from your MS-CHAP account. Must match the configuration of your RADIUS server.
  name: eapPwd
  type: string
- description: Indicates if the network doesn't broadcast its SSID. Mandatory for Android terminals, because these terminals rely on this setting to be able to connect to any network.
  name: hiddenSsid
  type: boolean
- description: Your name for the Wi-Fi profile.
  name: name
  type: string
- description: For `authType` **wpa-psk or **wpa2-psk**. The password to the wireless network.
  name: psk
  type: string
- description: The name of the wireless network.
  name: ssid
  type: string
- description: 'The type of encryption. Possible values: **auto**, **ccmp** (recommended), **tkip**'
  name: wsec
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-profile-schema.json
slug: management-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-profile-schema.json\",\n  \"title\": \"Profile\",\n  \"description\": \"Profile schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authType\": {\n      \"description\": \"The type of Wi-Fi network. Possible values: **wpa-psk**, **wpa2-psk**, **wpa-eap**, **wpa2-eap**.\",\n      \"type\": \"string\"\n    },\n    \"autoWifi\": {\n      \"description\": \"Indicates whether to automatically select the best authentication method available. Does not work on older terminal models.\",\n      \"type\": \"boolean\"\n    },\n    \"bssType\": {\n      \"description\": \"Use **infra** for infrastructure-based networks. This applies to most networks. Use **adhoc** only if the communication is p2p-based between base stations.\",\n      \"type\": \"string\"\n    },\n    \"channel\": {\n   \
  \   \"description\": \"The channel number of the Wi-Fi network. The recommended setting is **0** for automatic channel selection.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"defaultProfile\": {\n      \"description\": \"Indicates whether this is your preferred wireless network. If **true**, the terminal will try connecting to this network first.\",\n      \"type\": \"boolean\"\n    },\n    \"eap\": {\n      \"description\": \"For `authType` **wpa-eap** or **wpa2-eap**. Possible values: **tls**, **peap**, **leap**, **fast**\",\n      \"type\": \"string\"\n    },\n    \"eapCaCert\": {\n      \"description\": \"For `authType` **wpa-eap** or **wpa2-eap**. The root certificate from the CA that signed the certificate of the RADIUS server that is part of your wireless network.\",\n      \"$ref\": \"#/components/schemas/File\"\n    },\n    \"eapClientCert\": {\n      \"description\": \"For `eap` **tls**. The certificate chain for the terminals. All terminals in\
  \ the same network will use the same EAP client certificate.\",\n      \"$ref\": \"#/components/schemas/File\"\n    },\n    \"eapClientKey\": {\n      \"description\": \"For `eap` **tls**. The RSA private key for the client. Include the lines BEGIN RSA PRIVATE KEY and END RSA PRIVATE KEY.\",\n      \"$ref\": \"#/components/schemas/File\"\n    },\n    \"eapClientPwd\": {\n      \"description\": \"For `eap` **tls**. The password of the RSA key file, if that file is password-protected.\",\n      \"type\": \"string\"\n    },\n    \"eapIdentity\": {\n      \"description\": \"For `authType` **wpa-eap** or **wpa2-eap**. The EAP-PEAP username from your MS-CHAP account. Must match the configuration of your RADIUS server.\",\n      \"type\": \"string\"\n    },\n    \"eapIntermediateCert\": {\n      \"description\": \"For `eap` **tls**. The EAP intermediate certificate.\",\n      \"$ref\": \"#/components/schemas/File\"\n    },\n    \"eapPwd\": {\n      \"description\": \"For `eap` **peap**. The EAP-PEAP\
  \ password from your MS-CHAP account. Must match the configuration of your RADIUS server.\",\n      \"type\": \"string\"\n    },\n    \"hiddenSsid\": {\n      \"description\": \"Indicates if the network doesn't broadcast its SSID. Mandatory for Android terminals, because these terminals rely on this setting to be able to connect to any network.\",\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"description\": \"Your name for the Wi-Fi profile.\",\n      \"type\": \"string\"\n    },\n    \"psk\": {\n      \"description\": \"For `authType` **wpa-psk or **wpa2-psk**. The password to the wireless network.\",\n      \"type\": \"string\"\n    },\n    \"ssid\": {\n      \"description\": \"The name of the wireless network.\",\n      \"type\": \"string\"\n    },\n    \"wsec\": {\n      \"description\": \"The type of encryption. Possible values: **auto**, **ccmp** (recommended), **tkip**\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"ssid\",\n    \"bssType\"\
  ,\n    \"authType\",\n    \"wsec\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-profile-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Profile
---
