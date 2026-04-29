---
description: DeviceAuthorizationResponse from GitLab API
layout: schema
name: DeviceAuthorizationResponse
properties_list:
- description: The device verification code used to poll for the access token.
  name: device_code
  type: string
- description: The end-user verification code to enter on the authorization page.
  name: user_code
  type: string
- description: The end-user verification URI on the authorization server.
  name: verification_uri
  type: string
- description: The verification URI that includes the user_code.
  name: verification_uri_complete
  type: string
- description: The lifetime in seconds of the device_code and user_code.
  name: expires_in
  type: integer
- description: Minimum number of seconds between polling requests.
  name: interval
  type: integer
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-oauth2-device-authorization-response-schema.json
slug: gitlab-oauth2-device-authorization-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-device-authorization-response-schema.json\",\n  \"title\": \"DeviceAuthorizationResponse\",\n  \"description\": \"DeviceAuthorizationResponse from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"device_code\": {\n      \"type\": \"string\",\n      \"description\": \"The device verification code used to poll for the access token.\",\n      \"example\": \"example_value\"\n    },\n    \"user_code\": {\n      \"type\": \"string\",\n      \"description\": \"The end-user verification code to enter on the authorization page.\",\n      \"example\": \"example_value\"\n    },\n    \"verification_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The end-user verification URI on the authorization server.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\
  \n    },\n    \"verification_uri_complete\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The verification URI that includes the user_code.\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"The lifetime in seconds of the device_code and user_code.\",\n      \"example\": 42\n    },\n    \"interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of seconds between polling requests.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-device-authorization-response-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: DeviceAuthorizationResponse
---
