---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint. OAuth2 client credentials request See https://datatracker.ietf.org/doc/html/rfc6749#section-4.4
layout: schema
name: OAuthClientCredentialsRequest
properties_list:
- description: ''
  name: grant_type
  type: string
- description: ''
  name: scope
  type: string
- description: Client ID This can be sent in the request body, but OAuth2 recommends sending it in a Basic Authorization header.
  name: client_id
  type: string
- description: Client secret This can be sent in the request body, but OAuth2 recommends sending it in a Basic Authorization header.
  name: client_secret
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-client-credentials-request-schema.json
slug: rest-catalog-open-api-o-auth-client-credentials-request
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthClientCredentialsRequest
---
