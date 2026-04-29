---
description: WS-Security configuration properties for Apache CXF WSS4J interceptors.
layout: schema
name: WsSecurityConfig
properties_list:
- description: Space-separated list of WS-Security actions to apply.
  name: action
  type: string
- description: Password encoding type for UsernameToken.
  name: passwordType
  type: string
- description: Username for UsernameToken or keystore alias.
  name: user
  type: string
- description: Fully qualified class name of the javax.security.auth.callback.CallbackHandler for password retrieval.
  name: passwordCallbackClass
  type: string
- description: Key identifier type for XML Signature.
  name: signatureKeyIdentifier
  type: string
- description: Path to the signature keystore properties file.
  name: signaturePropFile
  type: string
- description: Path to the encryption keystore properties file.
  name: encryptionPropFile
  type: string
- description: Alias of the recipient public key for encryption.
  name: encryptionUser
  type: string
provider_name: Apache CXF
provider_slug: apache-cxf
schema_file: json-schema/apache-cxf-ws-security-config-schema.json
slug: apache-cxf-ws-security-config
source_filename: apache-cxf-ws-security-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-cxf/refs/heads/main/json-schema/apache-cxf-ws-security-config-schema.json\",\n  \"title\": \"WsSecurityConfig\",\n  \"description\": \"WS-Security configuration properties for Apache CXF WSS4J interceptors.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"Space-separated list of WS-Security actions to apply.\",\n      \"example\": \"UsernameToken Timestamp\"\n    },\n    \"passwordType\": {\n      \"type\": \"string\",\n      \"description\": \"Password encoding type for UsernameToken.\",\n      \"enum\": [\n        \"PasswordDigest\",\n        \"PasswordText\"\n      ],\n      \"example\": \"PasswordDigest\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"Username for UsernameToken or keystore alias.\",\n      \"example\": \"serviceUser\"\
  \n    },\n    \"passwordCallbackClass\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified class name of the javax.security.auth.callback.CallbackHandler for password retrieval.\",\n      \"example\": \"com.example.PasswordCallbackHandler\"\n    },\n    \"signatureKeyIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"Key identifier type for XML Signature.\",\n      \"enum\": [\n        \"IssuerSerial\",\n        \"DirectReference\",\n        \"X509KeyIdentifier\",\n        \"SKIKeyIdentifier\",\n        \"Thumbprint\"\n      ],\n      \"example\": \"IssuerSerial\"\n    },\n    \"signaturePropFile\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the signature keystore properties file.\",\n      \"example\": \"keystore.properties\"\n    },\n    \"encryptionPropFile\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the encryption keystore properties file.\",\n      \"example\": \"keystore.properties\"\n    },\n\
  \    \"encryptionUser\": {\n      \"type\": \"string\",\n      \"description\": \"Alias of the recipient public key for encryption.\",\n      \"example\": \"serverPublicKey\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-cxf/refs/heads/main/json-schema/apache-cxf-ws-security-config-schema.json
tags:
- Apache
- JAX-RS
- JAX-WS
- Java
- Open Source
- REST
- SOAP
- WS-Security
- Web Services
title: WsSecurityConfig
---
