---
description: DeviceAuthorizationRequest from GitLab API
layout: schema
name: DeviceAuthorizationRequest
properties_list:
- description: The application ID registered in GitLab.
  name: client_id
  type: string
- description: Space-separated list of requested scopes.
  name: scope
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-oauth2-device-authorization-request-schema.json
slug: gitlab-oauth2-device-authorization-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-device-authorization-request-schema.json\",\n  \"title\": \"DeviceAuthorizationRequest\",\n  \"description\": \"DeviceAuthorizationRequest from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID registered in GitLab.\",\n      \"example\": \"123456\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Space-separated list of requested scopes.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"client_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-device-authorization-request-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: DeviceAuthorizationRequest
---
