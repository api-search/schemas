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
