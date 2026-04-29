---
description: Response containing a list of SIP peers
layout: schema
name: SipPeerListResponse
properties_list:
- description: ''
  name: sipPeers
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/phone-numbers-sip-peer-list-response-schema.json
slug: phone-numbers-sip-peer-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-sip-peer-list-response-schema.json\",\n  \"title\": \"SipPeerListResponse\",\n  \"description\": \"Response containing a list of SIP peers\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sipPeers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SipPeer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/phone-numbers-sip-peer-list-response-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: SipPeerListResponse
---
