---
description: Groups of organization members that gives permissions on specified repositories.
layout: schema
name: nullable-team-simple
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
  name: members_url
  type: string
- description: Name of the team
  name: name
  type: string
- description: Description of the team
  name: description
  type: string
- description: Permission that the team will have for its repositories
  name: permission
  type: string
- description: The level of privacy this team should have
  name: privacy
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: repositories_url
  type: string
- description: ''
  name: slug
  type: string
- description: Distinguished Name (DN) that team maps to within LDAP environment
  name: ldap_dn
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-branches-api-nullable-team-simple-schema.json
slug: github-repo-branches-api-nullable-team-simple
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-branches-api-nullable-team-simple-schema.json\",\n  \"title\": \"nullable-team-simple\",\n  \"description\": \"Groups of organization members that gives permissions on specified repositories.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the team\",\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDQ6VGVhbTE=\"\n    },\n    \"url\": {\n      \"description\": \"URL for the team\",\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/1\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/organizations/1/team/1/members{/member}\"\n  \
  \  },\n    \"name\": {\n      \"description\": \"Name of the team\",\n      \"type\": \"string\",\n      \"example\": \"Justice League\"\n    },\n    \"description\": {\n      \"description\": \"Description of the team\",\n      \"type\": \"string\",\n      \"example\": \"great team.\"\n    },\n    \"permission\": {\n      \"description\": \"Permission that the team will have for its repositories\",\n      \"type\": \"string\",\n      \"example\": \"admin\"\n    },\n    \"privacy\": {\n      \"description\": \"The level of privacy this team should have\",\n      \"type\": \"string\",\n      \"example\": \"closed\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/orgs/rails/teams/core\"\n    },\n    \"repositories_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/organizations/1/team/1/repos\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n \
  \     \"example\": \"justice-league\"\n    },\n    \"ldap_dn\": {\n      \"description\": \"Distinguished Name (DN) that team maps to within LDAP environment\",\n      \"example\": \"uid=example,ou=users,dc=github,dc=com\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"url\",\n    \"members_url\",\n    \"name\",\n    \"description\",\n    \"permission\",\n    \"html_url\",\n    \"repositories_url\",\n    \"slug\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-branches-api-nullable-team-simple-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: nullable-team-simple
---
