---
description: A Client SSL profile for managing SSL/TLS connections between clients and the BIG-IP system.
layout: schema
name: ClientSslProfile
properties_list:
- description: ''
  name: kind
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: fullPath
  type: string
- description: ''
  name: generation
  type: integer
- description: ''
  name: selfLink
  type: string
- description: Alert timeout for SSL handshake.
  name: alertTimeout
  type: string
- description: Whether to allow non-SSL connections.
  name: allowNonSsl
  type: string
- description: Path to the SSL certificate file.
  name: cert
  type: string
- description: Certificate and key chain pairs.
  name: certKeyChain
  type: array
- description: Cipher suite string.
  name: ciphers
  type: string
- description: Parent profile.
  name: defaultsFrom
  type: string
- description: ''
  name: description
  type: string
- description: Path to the SSL private key file.
  name: key
  type: string
- description: SSL options.
  name: options
  type: array
- description: Client certificate verification mode.
  name: peerCertMode
  type: string
- description: Whether SSL renegotiation is allowed.
  name: renegotiation
  type: string
- description: Secure renegotiation mode.
  name: secureRenegotiation
  type: string
- description: Whether this is the default SNI profile.
  name: sniDefault
  type: string
- description: Whether SNI is required.
  name: sniRequire
  type: string
- description: Whether SSL forward proxy is enabled.
  name: sslForwardProxy
  type: string
- description: How to handle unclean SSL shutdowns.
  name: uncleanShutdown
  type: string
provider_name: F5 Networks
provider_slug: f5-networks
schema_file: json-schema/bigip-icontrol-rest-client-ssl-profile-schema.json
slug: bigip-icontrol-rest-client-ssl-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientSslProfile\",\n  \"type\": \"object\",\n  \"description\": \"A Client SSL profile for managing SSL/TLS connections between clients and the BIG-IP system.\",\n  \"properties\": {\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"fullPath\": {\n      \"type\": \"string\"\n    },\n    \"generation\": {\n      \"type\": \"integer\"\n    },\n    \"selfLink\": {\n      \"type\": \"string\"\n    },\n    \"alertTimeout\": {\n      \"type\": \"string\",\n      \"description\": \"Alert timeout for SSL handshake.\"\n    },\n    \"allowNonSsl\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to allow non-SSL connections.\"\n    },\n    \"cert\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the SSL certificate file.\"\n    },\n    \"certKeyChain\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Certificate and key chain pairs.\"\n    },\n    \"ciphers\": {\n      \"type\": \"string\",\n      \"description\": \"Cipher suite string.\"\n    },\n    \"defaultsFrom\": {\n      \"type\": \"string\",\n      \"description\": \"Parent profile.\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the SSL private key file.\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"description\": \"SSL options.\"\n    },\n    \"peerCertMode\": {\n      \"type\": \"string\",\n      \"description\": \"Client certificate verification mode.\"\n    },\n    \"renegotiation\": {\n      \"type\": \"string\",\n      \"description\": \"Whether SSL renegotiation is allowed.\"\n    },\n    \"secureRenegotiation\": {\n      \"type\": \"string\",\n      \"description\": \"Secure renegotiation mode.\"\n    },\n    \"sniDefault\": {\n      \"type\": \"string\",\n      \"description\": \"Whether this\
  \ is the default SNI profile.\"\n    },\n    \"sniRequire\": {\n      \"type\": \"string\",\n      \"description\": \"Whether SNI is required.\"\n    },\n    \"sslForwardProxy\": {\n      \"type\": \"string\",\n      \"description\": \"Whether SSL forward proxy is enabled.\"\n    },\n    \"uncleanShutdown\": {\n      \"type\": \"string\",\n      \"description\": \"How to handle unclean SSL shutdowns.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/f5-networks/refs/heads/main/json-schema/bigip-icontrol-rest-client-ssl-profile-schema.json
tags:
- API Gateway
- Application Delivery
- Automation
- Edge Computing
- Kubernetes
- Load Balancing
- Multi-Cloud
- NGINX
- Security
- WAF
title: ClientSslProfile
---
