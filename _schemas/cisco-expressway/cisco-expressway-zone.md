---
description: Schema for a zone configuration on Cisco Expressway. Zones define connections to external systems for call routing and firewall traversal. Supported zone types include Neighbor, TraversalClient, TraversalServer, DNS, ENUM, and Webex.
layout: schema
name: Cisco Expressway Zone
properties_list:
- description: Unique name for the zone
  name: Name
  type: string
- description: Zone type classification. Cannot be changed after creation.
  name: Type
  type: string
- description: Maximum number of times a search request can be forwarded through this zone. The lower of this value and any hop count already assigned to the request is used.
  name: HopCount
  type: integer
- description: Controls authentication challenge behavior for incoming messages from this zone
  name: AuthenticationPolicy
  type: string
- description: Media encryption enforcement mode for calls through this zone
  name: MediaEncryptionMode
  type: string
- description: ICE (Interactive Connectivity Establishment) message handling mode
  name: ICESupport
  type: string
- description: Whether H.323 protocol calls are enabled for this zone
  name: H323Mode
  type: string
- description: Port number for H.323 communication
  name: H323Port
  type: integer
- description: Whether SIP protocol calls are enabled for this zone
  name: SIPMode
  type: string
- description: Port number for SIP communication
  name: SIPPort
  type: integer
- description: Transport protocol for SIP messages
  name: SIPTransport
  type: string
- description: Whether to verify X.509 TLS certificates from the peer system
  name: SIPTLSVerifyMode
  type: string
- description: IP addresses or FQDNs of peer systems. Multiple peers are required for clusters (up to 6). Applicable to Neighbor and TraversalClient zones.
  name: PeerAddresses
  type: array
- description: Method for discovering peer addresses. Applicable to Neighbor zones.
  name: LookUpPeersBy
  type: string
- description: Preconfigured profile for specific peer system types. Sets multiple advanced settings automatically. Applicable to Neighbor zones.
  name: ZoneProfile
  type: string
- description: Username for traversal zone authentication. Must match between client and server configurations.
  name: ConnectionCredentialsUsername
  type: string
- description: Password for traversal zone authentication. Applicable to TraversalClient zones.
  name: ConnectionCredentialsPassword
  type: string
- description: Firewall traversal protocol for H.323. Applicable to traversal zones.
  name: H323Protocol
  type: string
- description: Whether Mobile and Remote Access (MRA) services are enabled. Applicable to TraversalServer zones.
  name: UnifiedCommunicationsMode
  type: string
- description: Certificate subject name for mutual TLS authentication. Must be FQDN for clustered clients. Applicable to TraversalServer zones.
  name: TLSVerifySubjectName
  type: string
- description: Determines media port sharing across multiple calls. Applicable to TraversalServer zones.
  name: H46019DemultiplexingMode
  type: string
- description: Frequency in seconds of retry attempts for failed connections. Applicable to TraversalClient zones.
  name: RetryInterval
  type: integer
- description: Frequency in seconds of SIP OPTIONS ping disconnection during failures. Applicable to TraversalClient zones.
  name: DisconnectOnFailInterval
  type: integer
- description: Whether to mark outbound requests to prevent reprocessing if returned. Applicable to TraversalClient zones.
  name: SIPPoisonMode
  type: string
- description: Whether multistream call negotiation is permitted. Applicable to Neighbor zones.
  name: MultistreamMode
  type: string
- description: Controls Route header processing in SIP INVITE requests. Applicable to Neighbor zones.
  name: PreloadedSipRoutesSupport
  type: string
- description: Whether P-Asserted-Identity headers from this zone are trusted. Applicable to Neighbor zones.
  name: SIPAuthenticationTrustMode
  type: string
- description: Whether to monitor the peer using H.323 LRQs and SIP OPTIONS. Applicable to Neighbor zones.
  name: MonitorPeerStatus
  type: string
- description: Default transport when DNS records do not specify preference. Applicable to DNS zones.
  name: FallbackTransportProtocol
  type: string
- description: Whether to route calls to a manually specified SIP domain. Applicable to DNS zones.
  name: ModifyDnsRequest
  type: string
- description: Whether to query A/AAAA records if SRV/NAPTR lookups fail. Applicable to DNS zones.
  name: IncludeAddressRecord
  type: string
- description: Domain appended to E.164 numbers for ENUM DNS lookups. Applicable to ENUM zones.
  name: DNSSuffix
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-zone-schema.json
slug: cisco-expressway-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-zone-schema.json\",\n  \"title\": \"Cisco Expressway Zone\",\n  \"description\": \"Schema for a zone configuration on Cisco Expressway. Zones define connections to external systems for call routing and firewall traversal. Supported zone types include Neighbor, TraversalClient, TraversalServer, DNS, ENUM, and Webex.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the zone\",\n      \"minLength\": 1,\n      \"maxLength\": 50,\n      \"examples\": [\"CUCM-Neighbor\", \"CEtoEXPE-Traversal\"]\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Zone type classification. Cannot be changed after creation.\",\n      \"enum\": [\"Neighbor\", \"TraversalClient\", \"TraversalServer\", \"DNS\", \"ENUM\", \"Webex\"]\n\
  \    },\n    \"HopCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of times a search request can be forwarded through this zone. The lower of this value and any hop count already assigned to the request is used.\",\n      \"minimum\": 0,\n      \"maximum\": 255,\n      \"default\": 15\n    },\n    \"AuthenticationPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Controls authentication challenge behavior for incoming messages from this zone\",\n      \"enum\": [\"DoNotCheckCredentials\", \"TreatAsAuthenticated\", \"CheckCredentials\"]\n    },\n    \"MediaEncryptionMode\": {\n      \"type\": \"string\",\n      \"description\": \"Media encryption enforcement mode for calls through this zone\",\n      \"enum\": [\"Force encrypted\", \"Force unencrypted\", \"Best effort\", \"Auto\"],\n      \"default\": \"Auto\"\n    },\n    \"ICESupport\": {\n      \"type\": \"string\",\n      \"description\": \"ICE (Interactive Connectivity Establishment)\
  \ message handling mode\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"H323Mode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether H.323 protocol calls are enabled for this zone\",\n      \"enum\": [\"On\", \"Off\"]\n    },\n    \"H323Port\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number for H.323 communication\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"SIPMode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether SIP protocol calls are enabled for this zone\",\n      \"enum\": [\"On\", \"Off\"]\n    },\n    \"SIPPort\": {\n      \"type\": \"integer\",\n      \"description\": \"Port number for SIP communication\",\n      \"minimum\": 1,\n      \"maximum\": 65535\n    },\n    \"SIPTransport\": {\n      \"type\": \"string\",\n      \"description\": \"Transport protocol for SIP messages\",\n      \"enum\": [\"TLS\", \"TCP\", \"UDP\"],\n      \"default\": \"TLS\"\n    },\n    \"\
  SIPTLSVerifyMode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to verify X.509 TLS certificates from the peer system\",\n      \"enum\": [\"On\", \"Off\"]\n    },\n    \"PeerAddresses\": {\n      \"type\": \"array\",\n      \"description\": \"IP addresses or FQDNs of peer systems. Multiple peers are required for clusters (up to 6). Applicable to Neighbor and TraversalClient zones.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1,\n      \"maxItems\": 6\n    },\n    \"LookUpPeersBy\": {\n      \"type\": \"string\",\n      \"description\": \"Method for discovering peer addresses. Applicable to Neighbor zones.\",\n      \"enum\": [\"Address\", \"Service record\"]\n    },\n    \"ZoneProfile\": {\n      \"type\": \"string\",\n      \"description\": \"Preconfigured profile for specific peer system types. Sets multiple advanced settings automatically. Applicable to Neighbor zones.\",\n      \"enum\": [\"Default\", \"Cisco Unified Communications\
  \ Manager\", \"Nortel Communication Server 1000\", \"Custom\"],\n      \"default\": \"Default\"\n    },\n    \"ConnectionCredentialsUsername\": {\n      \"type\": \"string\",\n      \"description\": \"Username for traversal zone authentication. Must match between client and server configurations.\"\n    },\n    \"ConnectionCredentialsPassword\": {\n      \"type\": \"string\",\n      \"description\": \"Password for traversal zone authentication. Applicable to TraversalClient zones.\"\n    },\n    \"H323Protocol\": {\n      \"type\": \"string\",\n      \"description\": \"Firewall traversal protocol for H.323. Applicable to traversal zones.\",\n      \"enum\": [\"Assent\", \"H.460.18\"],\n      \"default\": \"Assent\"\n    },\n    \"UnifiedCommunicationsMode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether Mobile and Remote Access (MRA) services are enabled. Applicable to TraversalServer zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n\
  \    \"TLSVerifySubjectName\": {\n      \"type\": \"string\",\n      \"description\": \"Certificate subject name for mutual TLS authentication. Must be FQDN for clustered clients. Applicable to TraversalServer zones.\"\n    },\n    \"H46019DemultiplexingMode\": {\n      \"type\": \"string\",\n      \"description\": \"Determines media port sharing across multiple calls. Applicable to TraversalServer zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"RetryInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Frequency in seconds of retry attempts for failed connections. Applicable to TraversalClient zones.\",\n      \"default\": 120\n    },\n    \"DisconnectOnFailInterval\": {\n      \"type\": \"integer\",\n      \"description\": \"Frequency in seconds of SIP OPTIONS ping disconnection during failures. Applicable to TraversalClient zones.\",\n      \"default\": 120\n    },\n    \"SIPPoisonMode\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Whether to mark outbound requests to prevent reprocessing if returned. Applicable to TraversalClient zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"MultistreamMode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether multistream call negotiation is permitted. Applicable to Neighbor zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"PreloadedSipRoutesSupport\": {\n      \"type\": \"string\",\n      \"description\": \"Controls Route header processing in SIP INVITE requests. Applicable to Neighbor zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"SIPAuthenticationTrustMode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether P-Asserted-Identity headers from this zone are trusted. Applicable to Neighbor zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"MonitorPeerStatus\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Whether to monitor the peer using H.323 LRQs and SIP OPTIONS. Applicable to Neighbor zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"On\"\n    },\n    \"FallbackTransportProtocol\": {\n      \"type\": \"string\",\n      \"description\": \"Default transport when DNS records do not specify preference. Applicable to DNS zones.\",\n      \"enum\": [\"TLS\", \"TCP\", \"UDP\"],\n      \"default\": \"TLS\"\n    },\n    \"ModifyDnsRequest\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to route calls to a manually specified SIP domain. Applicable to DNS zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"Off\"\n    },\n    \"IncludeAddressRecord\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to query A/AAAA records if SRV/NAPTR lookups fail. Applicable to DNS zones.\",\n      \"enum\": [\"On\", \"Off\"],\n      \"default\": \"On\"\n    },\n    \"DNSSuffix\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Domain appended to E.164 numbers for ENUM DNS lookups. Applicable to ENUM zones.\"\n    }\n  },\n  \"required\": [\"Name\", \"Type\"],\n  \"allOf\": [\n    {\n      \"if\": {\n        \"properties\": { \"Type\": { \"const\": \"Neighbor\" } }\n      },\n      \"then\": {\n        \"required\": [\"PeerAddresses\"]\n      }\n    },\n    {\n      \"if\": {\n        \"properties\": { \"Type\": { \"const\": \"TraversalClient\" } }\n      },\n      \"then\": {\n        \"required\": [\"PeerAddresses\", \"ConnectionCredentialsUsername\", \"ConnectionCredentialsPassword\"]\n      }\n    },\n    {\n      \"if\": {\n        \"properties\": { \"Type\": { \"const\": \"TraversalServer\" } }\n      },\n      \"then\": {\n        \"required\": [\"ConnectionCredentialsUsername\"]\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-zone-schema.json
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Zone
---
