---
description: A GitHub organization that groups users and repositories together under shared ownership, permissions, and policies.
layout: schema
name: GitHub Organization
properties_list:
- description: The login name of the organization.
  name: login
  type: string
- description: The unique identifier of the organization.
  name: id
  type: integer
- description: The GraphQL node ID for the organization.
  name: node_id
  type: string
- description: The API URL for the organization.
  name: url
  type: string
- description: The URL of the organization on GitHub.
  name: html_url
  type: string
- description: API URL for the organization's repositories.
  name: repos_url
  type: string
- description: API URL for the organization's events.
  name: events_url
  type: string
- description: API URL for the organization's webhooks.
  name: hooks_url
  type: string
- description: API URL for the organization's issues.
  name: issues_url
  type: string
- description: API URL template for the organization's members.
  name: members_url
  type: string
- description: API URL template for the organization's public members.
  name: public_members_url
  type: string
- description: URL to the organization's avatar image.
  name: avatar_url
  type: string
- description: A description of the organization.
  name: description
  type:
  - string
  - 'null'
- description: The display name of the organization.
  name: name
  type:
  - string
  - 'null'
- description: The company name associated with the organization.
  name: company
  type:
  - string
  - 'null'
- description: The organization's blog or website URL.
  name: blog
  type:
  - string
  - 'null'
- description: The organization's location.
  name: location
  type:
  - string
  - 'null'
- description: The organization's publicly visible email address.
  name: email
  type:
  - string
  - 'null'
- description: The organization's Twitter/X username.
  name: twitter_username
  type:
  - string
  - 'null'
- description: Whether the organization has verified its domain.
  name: is_verified
  type: boolean
- description: Whether the organization has projects enabled.
  name: has_organization_projects
  type: boolean
- description: Whether repositories can have projects enabled.
  name: has_repository_projects
  type: boolean
- description: The number of public repositories.
  name: public_repos
  type: integer
- description: The number of public gists.
  name: public_gists
  type: integer
- description: The number of followers.
  name: followers
  type: integer
- description: The number of users the organization is following.
  name: following
  type: integer
- description: The account type.
  name: type
  type: string
- description: The date and time the organization was created.
  name: created_at
  type: string
- description: The date and time the organization was last updated.
  name: updated_at
  type: string
- description: ''
  name: plan
  type: object
- description: The default permission level for new repositories.
  name: default_repository_permission
  type: string
- description: Whether members can create repositories.
  name: members_can_create_repositories
  type: boolean
- description: Whether members can create public repositories.
  name: members_can_create_public_repositories
  type: boolean
- description: Whether members can create private repositories.
  name: members_can_create_private_repositories
  type: boolean
- description: Whether two-factor authentication is required for members.
  name: two_factor_requirement_enabled
  type: boolean
- description: The total number of private repositories.
  name: total_private_repos
  type: integer
- description: The number of private repositories owned by the organization.
  name: owned_private_repos
  type: integer
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-organization-schema.json
slug: github-organization
source_filename: github-organization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/schemas/github/organization.json\",\n  \"title\": \"GitHub Organization\",\n  \"description\": \"A GitHub organization that groups users and repositories together under shared ownership, permissions, and policies.\",\n  \"type\": \"object\",\n  \"required\": [\"login\", \"id\"],\n  \"properties\": {\n    \"login\": {\n      \"type\": \"string\",\n      \"description\": \"The login name of the organization.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the organization.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID for the organization.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the organization.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\"\
  ,\n      \"description\": \"The URL of the organization on GitHub.\"\n    },\n    \"repos_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for the organization's repositories.\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for the organization's events.\"\n    },\n    \"hooks_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for the organization's webhooks.\"\n    },\n    \"issues_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for the organization's issues.\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"description\": \"API URL template for the organization's members.\"\n    },\n    \"public_members_url\": {\n      \"type\": \"string\",\n      \"description\": \"API URL template for the organization's public members.\"\n    },\n    \"\
  avatar_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the organization's avatar image.\"\n    },\n    \"description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A description of the organization.\"\n    },\n    \"name\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The display name of the organization.\"\n    },\n    \"company\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The company name associated with the organization.\"\n    },\n    \"blog\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The organization's blog or website URL.\"\n    },\n    \"location\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The organization's location.\"\n    },\n    \"email\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"email\",\n      \"description\": \"The organization's publicly visible email address.\"\n    },\n\
  \    \"twitter_username\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The organization's Twitter/X username.\"\n    },\n    \"is_verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization has verified its domain.\"\n    },\n    \"has_organization_projects\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the organization has projects enabled.\"\n    },\n    \"has_repository_projects\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether repositories can have projects enabled.\"\n    },\n    \"public_repos\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of public repositories.\"\n    },\n    \"public_gists\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of public gists.\"\n    },\n    \"followers\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of followers.\"\
  \n    },\n    \"following\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of users the organization is following.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"Organization\",\n      \"description\": \"The account type.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the organization was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the organization was last updated.\"\n    },\n    \"plan\": {\n      \"$ref\": \"#/$defs/Plan\"\n    },\n    \"default_repository_permission\": {\n      \"type\": \"string\",\n      \"enum\": [\"read\", \"write\", \"admin\", \"none\"],\n      \"description\": \"The default permission level for new repositories.\"\n    },\n    \"members_can_create_repositories\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether members can create repositories.\"\n    },\n    \"members_can_create_public_repositories\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether members can create public repositories.\"\n    },\n    \"members_can_create_private_repositories\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether members can create private repositories.\"\n    },\n    \"two_factor_requirement_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether two-factor authentication is required for members.\"\n    },\n    \"total_private_repos\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The total number of private repositories.\"\n    },\n    \"owned_private_repos\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"The number of private repositories owned by the organization.\"\n    }\n  },\n  \"$defs\": {\n    \"Plan\": {\n      \"type\": \"object\",\n      \"\
  description\": \"The billing plan for the organization.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the plan.\"\n        },\n        \"space\": {\n          \"type\": \"integer\",\n          \"description\": \"The amount of disk space available in KB.\"\n        },\n        \"private_repos\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of private repos allowed.\"\n        },\n        \"filled_seats\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of filled seats.\"\n        },\n        \"seats\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of seats available.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organization-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: GitHub Organization
---
