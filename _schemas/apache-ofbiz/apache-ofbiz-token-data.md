---
description: JWT token data returned after successful authentication.
layout: schema
name: TokenData
properties_list:
- description: JWT access token for Bearer authentication.
  name: access_token
  type: string
- description: Token type, always Bearer.
  name: token_type
  type: string
- description: Token expiry duration in seconds.
  name: expires_in
  type: string
- description: Refresh token for obtaining new access tokens.
  name: refresh_token
  type: string
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-token-data-schema.json
slug: apache-ofbiz-token-data
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: TokenData
---
