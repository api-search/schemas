---
description: Groups of organization members that gives permissions on specified repositories.
layout: schema
name: team-full
properties_list:
- description: Unique identifier of the team
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: URL for the team
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: Name of the team
  name: name
  type: string
- description: ''
  name: slug
  type: string
- description: ''
  name: description
  type: string
- description: The level of privacy this team should have
  name: privacy
  type: string
- description: Permission that the team will have for its repositories
  name: permission
  type: string
- description: ''
  name: members_url
  type: string
- description: ''
  name: repositories_url
  type: string
- description: ''
  name: parent
  type: object
- description: ''
  name: members_count
  type: integer
- description: ''
  name: repos_count
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: organization
  type: object
- description: Distinguished Name (DN) that team maps to within LDAP environment
  name: ldap_dn
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-teams-team-full-schema.json
slug: github-teams-team-full
source_filename: github-teams-team-full-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-full-schema.json\",\n  \"title\": \"team-full\",\n  \"description\": \"Groups of organization members that gives permissions on specified repositories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the team\",\n      \"example\": 42,\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDQ6VGVhbTE=\"\n    },\n    \"url\": {\n      \"description\": \"URL for the team\",\n      \"example\": \"https://api.github.com/organizations/1/team/1\",\n      \"type\": \"string\",\n      \"format\": \"uri\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/orgs/rails/teams/core\"\n    },\n    \"name\": {\n      \"\
  description\": \"Name of the team\",\n      \"example\": \"Developers\",\n      \"type\": \"string\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"example\": \"justice-league\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A great team.\",\n      \"nullable\": true\n    },\n    \"privacy\": {\n      \"description\": \"The level of privacy this team should have\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"closed\",\n        \"secret\"\n      ],\n      \"example\": \"closed\"\n    },\n    \"permission\": {\n      \"description\": \"Permission that the team will have for its repositories\",\n      \"example\": \"push\",\n      \"type\": \"string\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/organizations/1/team/1/members{/member}\"\n    },\n    \"repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/1/repos\"\
  \n    },\n    \"parent\": {\n      \"$ref\": \"#/components/schemas/nullable-team-simple\"\n    },\n    \"members_count\": {\n      \"type\": \"integer\",\n      \"example\": 3\n    },\n    \"repos_count\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-07-14T16:53:42Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2017-08-17T12:37:15Z\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/team-organization\"\n    },\n    \"ldap_dn\": {\n      \"description\": \"Distinguished Name (DN) that team maps to within LDAP environment\",\n      \"example\": \"uid=example,ou=users,dc=github,dc=com\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"url\",\n    \"members_url\",\n    \"name\",\n    \"description\",\n    \"permission\"\
  ,\n    \"html_url\",\n    \"repositories_url\",\n    \"slug\",\n    \"created_at\",\n    \"updated_at\",\n    \"members_count\",\n    \"repos_count\",\n    \"organization\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-team-full-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: team-full
---
