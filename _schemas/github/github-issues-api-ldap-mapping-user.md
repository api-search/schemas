---
description: Ldap Private User
layout: schema
name: ldap-mapping-user
properties_list:
- description: ''
  name: ldap_dn
  type: string
- description: ''
  name: login
  type: string
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: avatar_url
  type: string
- description: ''
  name: gravatar_id
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: followers_url
  type: string
- description: ''
  name: following_url
  type: string
- description: ''
  name: gists_url
  type: string
- description: ''
  name: starred_url
  type: string
- description: ''
  name: subscriptions_url
  type: string
- description: ''
  name: organizations_url
  type: string
- description: ''
  name: repos_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: received_events_url
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: site_admin
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: company
  type: string
- description: ''
  name: blog
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: hireable
  type: boolean
- description: ''
  name: bio
  type: string
- description: ''
  name: twitter_username
  type: string
- description: ''
  name: public_repos
  type: integer
- description: ''
  name: public_gists
  type: integer
- description: ''
  name: followers
  type: integer
- description: ''
  name: following
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: private_gists
  type: integer
- description: ''
  name: total_private_repos
  type: integer
- description: ''
  name: owned_private_repos
  type: integer
- description: ''
  name: disk_usage
  type: integer
- description: ''
  name: collaborators
  type: integer
- description: ''
  name: two_factor_authentication
  type: boolean
- description: ''
  name: plan
  type: object
- description: ''
  name: suspended_at
  type: string
- description: ''
  name: business_plus
  type: boolean
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-issues-api-ldap-mapping-user-schema.json
slug: github-issues-api-ldap-mapping-user
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-issues-api-ldap-mapping-user-schema.json\",\n  \"title\": \"ldap-mapping-user\",\n  \"description\": \"Ldap Private User\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ldap_dn\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"login\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDQ6VXNlcjE=\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/images/error/octocat_happy.gif\"\n    },\n    \"gravatar_id\": {\n      \"type\": \"string\",\n      \"example\": \"41d064eb2195891e12d0413f63227ea7\"\
  ,\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/octocat\"\n    },\n    \"followers_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/followers\"\n    },\n    \"following_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/following{/other_user}\"\n    },\n    \"gists_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/gists{/gist_id}\"\n    },\n    \"starred_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/starred{/owner}{/repo}\"\n    },\n    \"subscriptions_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"\
  example\": \"https://api.github.com/users/octocat/subscriptions\"\n    },\n    \"organizations_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/orgs\"\n    },\n    \"repos_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/repos\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/users/octocat/events{/privacy}\"\n    },\n    \"received_events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/users/octocat/received_events\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"User\"\n    },\n    \"site_admin\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"monalisa octocat\",\n      \"nullable\": true\n    },\n    \"\
  company\": {\n      \"type\": \"string\",\n      \"example\": \"GitHub\",\n      \"nullable\": true\n    },\n    \"blog\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/blog\",\n      \"nullable\": true\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\",\n      \"nullable\": true\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"octocat@github.com\",\n      \"nullable\": true\n    },\n    \"hireable\": {\n      \"type\": \"boolean\",\n      \"nullable\": true\n    },\n    \"bio\": {\n      \"type\": \"string\",\n      \"example\": \"There once was...\",\n      \"nullable\": true\n    },\n    \"twitter_username\": {\n      \"type\": \"string\",\n      \"example\": \"monalisa\",\n      \"nullable\": true\n    },\n    \"public_repos\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    },\n    \"public_gists\": {\n      \"type\": \"integer\",\n      \"example\"\
  : 1\n    },\n    \"followers\": {\n      \"type\": \"integer\",\n      \"example\": 20\n    },\n    \"following\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2008-01-14T04:33:35Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2008-01-14T04:33:35Z\"\n    },\n    \"private_gists\": {\n      \"type\": \"integer\",\n      \"example\": 81\n    },\n    \"total_private_repos\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"owned_private_repos\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"disk_usage\": {\n      \"type\": \"integer\",\n      \"example\": 10000\n    },\n    \"collaborators\": {\n      \"type\": \"integer\",\n      \"example\": 8\n    },\n    \"two_factor_authentication\": {\n      \"type\": \"boolean\",\n      \"example\": true\n  \
  \  },\n    \"plan\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"collaborators\": {\n          \"type\": \"integer\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"space\": {\n          \"type\": \"integer\"\n        },\n        \"private_repos\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"required\": [\n        \"collaborators\",\n        \"name\",\n        \"space\",\n        \"private_repos\"\n      ]\n    },\n    \"suspended_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true\n    },\n    \"business_plus\": {\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"avatar_url\",\n    \"events_url\",\n    \"followers_url\",\n    \"following_url\",\n    \"gists_url\",\n    \"gravatar_id\",\n    \"html_url\",\n    \"id\",\n    \"node_id\",\n    \"login\",\n    \"organizations_url\",\n    \"received_events_url\",\n    \"repos_url\",\n    \"site_admin\"\
  ,\n    \"starred_url\",\n    \"subscriptions_url\",\n    \"type\",\n    \"url\",\n    \"bio\",\n    \"blog\",\n    \"company\",\n    \"email\",\n    \"followers\",\n    \"following\",\n    \"hireable\",\n    \"location\",\n    \"name\",\n    \"public_gists\",\n    \"public_repos\",\n    \"created_at\",\n    \"updated_at\",\n    \"collaborators\",\n    \"disk_usage\",\n    \"owned_private_repos\",\n    \"private_gists\",\n    \"total_private_repos\",\n    \"two_factor_authentication\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-issues-api-ldap-mapping-user-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: ldap-mapping-user
---
