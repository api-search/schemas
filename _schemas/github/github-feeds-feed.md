---
description: Feed
layout: schema
name: feed
properties_list:
- description: ''
  name: timeline_url
  type: string
- description: ''
  name: user_url
  type: string
- description: ''
  name: current_user_public_url
  type: string
- description: ''
  name: current_user_url
  type: string
- description: ''
  name: current_user_actor_url
  type: string
- description: ''
  name: current_user_organization_url
  type: string
- description: ''
  name: current_user_organization_urls
  type: array
- description: ''
  name: security_advisories_url
  type: string
- description: A feed of discussions for a given repository.
  name: repository_discussions_url
  type: string
- description: A feed of discussions for a given repository and category.
  name: repository_discussions_category_url
  type: string
- description: ''
  name: _links
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-feeds-feed-schema.json
slug: github-feeds-feed
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-feeds-feed-schema.json\",\n  \"title\": \"feed\",\n  \"description\": \"Feed\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timeline_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/timeline\"\n    },\n    \"user_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/{user}\"\n    },\n    \"current_user_public_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/octocat\"\n    },\n    \"current_user_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/octocat.private?token=abc123\"\n    },\n    \"current_user_actor_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/octocat.private.actor?token=abc123\"\n    },\n    \"current_user_organization_url\": {\n      \"type\"\
  : \"string\",\n      \"example\": \"https://github.com/octocat-org\"\n    },\n    \"current_user_organization_urls\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"https://github.com/organizations/github/octocat.private.atom?token=abc123\"\n      ],\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"security_advisories_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/security-advisories\"\n    },\n    \"repository_discussions_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/{user}/{repo}/discussions\",\n      \"description\": \"A feed of discussions for a given repository.\"\n    },\n    \"repository_discussions_category_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/{user}/{repo}/discussions/categories/{category}\",\n      \"description\": \"A feed of discussions for a given repository and category.\"\n    },\n    \"_links\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"timeline\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"user\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"security_advisories\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"current_user\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"current_user_public\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"current_user_actor\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"current_user_organization\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"current_user_organizations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/components/schemas/link-with-type\"\n          }\n        },\n        \"repository_discussions\"\
  : {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        },\n        \"repository_discussions_category\": {\n          \"$ref\": \"#/components/schemas/link-with-type\"\n        }\n      },\n      \"required\": [\n        \"timeline\",\n        \"user\"\n      ]\n    }\n  },\n  \"required\": [\n    \"_links\",\n    \"timeline_url\",\n    \"user_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-feeds-feed-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: feed
---
