---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint. OAuth2 token exchange request See https://datatracker.ietf.org/doc/html/rfc8693
layout: schema
name: OAuthTokenExchangeRequest
properties_list:
- description: ''
  name: grant_type
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: requested_token_type
  type: object
- description: Subject token for token exchange request
  name: subject_token
  type: string
- description: ''
  name: subject_token_type
  type: object
- description: Actor token for token exchange request
  name: actor_token
  type: string
- description: ''
  name: actor_token_type
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-token-exchange-request-schema.json
slug: rest-catalog-open-api-o-auth-token-exchange-request
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthTokenExchangeRequest
---
