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
