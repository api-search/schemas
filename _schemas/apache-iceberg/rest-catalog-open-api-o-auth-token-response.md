---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.
layout: schema
name: OAuthTokenResponse
properties_list:
- description: The access token, for client credentials or token exchange
  name: access_token
  type: string
- description: Access token type for client credentials or token exchange See https://datatracker.ietf.org/doc/html/rfc6749#section-7.1
  name: token_type
  type: string
- description: Lifetime of the access token in seconds for client credentials or token exchange
  name: expires_in
  type: integer
- description: ''
  name: issued_token_type
  type: object
- description: Refresh token for client credentials or token exchange
  name: refresh_token
  type: string
- description: Authorization scope for client credentials or token exchange
  name: scope
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-token-response-schema.json
slug: rest-catalog-open-api-o-auth-token-response
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthTokenResponse
---
