---
description: A SIP peer (location) within a site
layout: schema
name: SipPeer
properties_list:
- description: The unique identifier for the SIP peer
  name: peerId
  type: string
- description: The name of the SIP peer
  name: peerName
  type: string
- description: A description of the SIP peer
  name: description
  type: string
- description: Whether this is the default SIP peer for the site
  name: isDefaultPeer
  type: boolean
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-sip-peer-schema.json
slug: phone-numbers-sip-peer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-sip-peer-schema.json\",\n  \"title\": \"SipPeer\",\n  \"description\": \"A SIP peer (location) within a site\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"peerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the SIP peer\"\n    },\n    \"peerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the SIP peer\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the SIP peer\"\n    },\n    \"isDefaultPeer\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the default SIP peer for the site\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-sip-peer-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: SipPeer
---
