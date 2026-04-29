---
description: ''
layout: schema
name: OidcCustomSub
properties_list:
- description: ''
  name: use_default
  type: boolean
- description: ''
  name: include_claim_keys
  type: array
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-oidc-custom-sub-schema.json
slug: github-actions-oidc-custom-sub
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OidcCustomSub\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"use_default\": {\n      \"type\": \"boolean\"\n    },\n    \"include_claim_keys\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-oidc-custom-sub-schema.json
tags: []
title: OidcCustomSub
---
