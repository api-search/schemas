---
description: The token response
layout: schema
name: AmadeusOAuth2Token
properties_list:
- description: The access token issued by the authorization server.
  name: type
  type: string
- description: The user who requested the access_token
  name: username
  type: string
- description: The application which is requested the access_token
  name: application_name
  type: string
- description: The client_id is a public identifier for apps
  name: client_id
  type: string
- description: token_type is a parameter in Access Token generate call to Authorization server, which essentially represents how an access_token will be generated and presented for resource access calls
  name: token_type
  type: string
- description: Access tokens are a String which applications use to make API requests on behalf of a user.
  name: access_token
  type: string
- description: The lifetime in seconds of the access token
  name: expires_in
  type: integer
- description: The state
  name: state
  type: string
- description: Scope is a mechanism in OAuth 2.0 to limit an application's access to a user's account
  name: scope
  type: string
provider_name: Amadeus
provider_slug: amadeus
schema_file: json-schema/amadeus-oauth2-login-amadeusoauth2token-schema.json
slug: amadeus-oauth2-login-amadeusoauth2token
tags:
- Airlines
- Aviation
- Booking
- Destinations
- Flights
- Hospitality
- Hotels
- Market Insights
- Tourism
- Transfers
- Travel
title: AmadeusOAuth2Token
---
