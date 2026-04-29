---
description: Security classification flags for the IP
layout: schema
name: IPSecurityFlags
properties_list:
- description: IP is a known VPN endpoint
  name: is_vpn
  type: boolean
- description: IP is a known proxy server
  name: is_proxy
  type: boolean
- description: IP is a Tor exit node
  name: is_tor
  type: boolean
- description: IP belongs to a hosting or cloud provider
  name: is_hosting
  type: boolean
- description: IP is used as a relay (e.g., Apple Private Relay)
  name: is_relay
  type: boolean
- description: IP is associated with a mobile network
  name: is_mobile
  type: boolean
- description: IP has been flagged for abuse
  name: is_abuse
  type: boolean
provider_name: Abstract API
provider_slug: abstract-api
schema_file: json-schema/ip-intelligence-ip-security-flags-schema.json
slug: ip-intelligence-ip-security-flags
source_filename: ip-intelligence-ip-security-flags-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-ip-security-flags-schema.json\",\n  \"title\": \"IPSecurityFlags\",\n  \"description\": \"Security classification flags for the IP\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"is_vpn\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP is a known VPN endpoint\",\n      \"example\": false\n    },\n    \"is_proxy\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP is a known proxy server\",\n      \"example\": false\n    },\n    \"is_tor\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP is a Tor exit node\",\n      \"example\": false\n    },\n    \"is_hosting\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP belongs to a hosting or cloud provider\",\n      \"example\": true\n    },\n    \"is_relay\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"IP is used as a relay (e.g., Apple Private Relay)\",\n      \"example\": false\n    },\n    \"is_mobile\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP is associated with a mobile network\",\n      \"example\": false\n    },\n    \"is_abuse\": {\n      \"type\": \"boolean\",\n      \"description\": \"IP has been flagged for abuse\",\n      \"example\": false\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abstract-api/refs/heads/main/json-schema/ip-intelligence-ip-security-flags-schema.json
tags:
- Avatars
- Company Enrichment
- Contacts
- Currencies
- Email Validation
- Exchange Rates
- IBAN Validation
- Image Processing
- IP Geolocation
- IP Intelligence
- Phone Validation
- Public Holidays
- Screenshots
- Timezones
- VAT Validation
- Web Scraping
title: IPSecurityFlags
---
