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
