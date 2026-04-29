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
source_filename: amadeus-oauth2-login-amadeusoauth2token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AmadeusOAuth2Token\",\n  \"description\": \"The token response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The access token issued by the authorization server.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The user who requested the access_token\"\n    },\n    \"application_name\": {\n      \"type\": \"string\",\n      \"description\": \"The application which is requested the access_token\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The client_id is a public identifier for apps\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"token_type is a parameter in Access Token generate call to Authorization server, which essentially represents how an access_token will be generated and presented for resource access\
  \ calls\"\n    },\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"Access tokens are a String which applications use to make API requests on behalf of a user.\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The lifetime in seconds of the access token\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Scope is a mechanism in OAuth 2.0 to limit an application's access to a user's account\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amadeus/refs/heads/main/json-schema/amadeus-oauth2-login-amadeusoauth2token-schema.json
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
