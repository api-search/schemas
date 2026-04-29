---
description: Organization Full
layout: schema
name: organization-full
properties_list:
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
  name: url
  type: string
- description: ''
  name: repos_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: hooks_url
  type: string
- description: ''
  name: issues_url
  type: string
- description: ''
  name: members_url
  type: string
- description: ''
  name: public_members_url
  type: string
- description: ''
  name: avatar_url
  type: string
- description: ''
  name: description
  type: string
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
  name: twitter_username
  type: string
- description: ''
  name: is_verified
  type: boolean
- description: ''
  name: has_organization_projects
  type: boolean
- description: ''
  name: has_repository_projects
  type: boolean
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
  name: html_url
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: total_private_repos
  type: integer
- description: ''
  name: owned_private_repos
  type: integer
- description: ''
  name: private_gists
  type: integer
- description: ''
  name: disk_usage
  type: integer
- description: ''
  name: collaborators
  type: integer
- description: ''
  name: billing_email
  type: string
- description: ''
  name: plan
  type: object
- description: ''
  name: default_repository_permission
  type: string
- description: ''
  name: members_can_create_repositories
  type: boolean
- description: ''
  name: two_factor_requirement_enabled
  type: boolean
- description: ''
  name: members_allowed_repository_creation_type
  type: string
- description: ''
  name: members_can_create_public_repositories
  type: boolean
- description: ''
  name: members_can_create_private_repositories
  type: boolean
- description: ''
  name: members_can_create_internal_repositories
  type: boolean
- description: ''
  name: members_can_create_pages
  type: boolean
- description: ''
  name: members_can_create_public_pages
  type: boolean
- description: ''
  name: members_can_create_private_pages
  type: boolean
- description: ''
  name: members_can_fork_private_repositories
  type: boolean
- description: ''
  name: web_commit_signoff_required
  type: boolean
- description: Whether GitHub Advanced Security is enabled for new repositories and repositories transferred to this organization. This field is only visible to organization owners or members of a team with the secu
  name: advanced_security_enabled_for_new_repositories
  type: boolean
- description: Whether GitHub Advanced Security is automatically enabled for new repositories and repositories transferred to this organization. This field is only visible to organization owners or members of a team
  name: dependabot_alerts_enabled_for_new_repositories
  type: boolean
- description: 'Whether dependabot security updates are automatically enabled for new repositories and repositories transferred to this organization. This field is only visible to organization owners or members of a '
  name: dependabot_security_updates_enabled_for_new_repositories
  type: boolean
- description: Whether dependency graph is automatically enabled for new repositories and repositories transferred to this organization. This field is only visible to organization owners or members of a team with th
  name: dependency_graph_enabled_for_new_repositories
  type: boolean
- description: Whether secret scanning is automatically enabled for new repositories and repositories transferred to this organization. This field is only visible to organization owners or members of a team with the
  name: secret_scanning_enabled_for_new_repositories
  type: boolean
- description: Whether secret scanning push protection is automatically enabled for new repositories and repositories transferred to this organization. This field is only visible to organization owners or members of
  name: secret_scanning_push_protection_enabled_for_new_repositories
  type: boolean
- description: Whether a custom link is shown to contributors who are blocked from pushing a secret by push protection.
  name: secret_scanning_push_protection_custom_link_enabled
  type: boolean
- description: An optional URL string to display to contributors who are blocked from pushing a secret.
  name: secret_scanning_push_protection_custom_link
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-organizations-organization-full-schema.json
slug: github-organizations-organization-full
source_filename: github-organizations-organization-full-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-organization-full-schema.json\",\n  \"title\": \"organization-full\",\n  \"description\": \"Organization Full\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"login\": {\n      \"type\": \"string\",\n      \"example\": \"github\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDEyOk9yZ2FuaXphdGlvbjE=\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/orgs/github\"\n    },\n    \"repos_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/orgs/github/repos\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n \
  \     \"example\": \"https://api.github.com/orgs/github/events\"\n    },\n    \"hooks_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/hooks\"\n    },\n    \"issues_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/issues\"\n    },\n    \"members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/members{/member}\"\n    },\n    \"public_members_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/orgs/github/public_members{/member}\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/images/error/octocat_happy.gif\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"A great organization\",\n      \"nullable\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"github\"\n    },\n    \"company\": {\n      \"type\":\
  \ \"string\",\n      \"example\": \"GitHub\"\n    },\n    \"blog\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/blog\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\": \"octocat@github.com\"\n    },\n    \"twitter_username\": {\n      \"type\": \"string\",\n      \"example\": \"github\",\n      \"nullable\": true\n    },\n    \"is_verified\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"has_organization_projects\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"has_repository_projects\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"public_repos\": {\n      \"type\": \"integer\",\n      \"example\": 2\n    },\n    \"public_gists\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"followers\"\
  : {\n      \"type\": \"integer\",\n      \"example\": 20\n    },\n    \"following\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/octocat\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"Organization\"\n    },\n    \"total_private_repos\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"owned_private_repos\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"private_gists\": {\n      \"type\": \"integer\",\n      \"example\": 81,\n      \"nullable\": true\n    },\n    \"disk_usage\": {\n      \"type\": \"integer\",\n      \"example\": 10000,\n      \"nullable\": true\n    },\n    \"collaborators\": {\n      \"type\": \"integer\",\n      \"example\": 8,\n      \"nullable\": true\n    },\n    \"billing_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"example\"\
  : \"org@example.com\",\n      \"nullable\": true\n    },\n    \"plan\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"space\": {\n          \"type\": \"integer\"\n        },\n        \"private_repos\": {\n          \"type\": \"integer\"\n        },\n        \"filled_seats\": {\n          \"type\": \"integer\"\n        },\n        \"seats\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"required\": [\n        \"name\",\n        \"space\",\n        \"private_repos\"\n      ]\n    },\n    \"default_repository_permission\": {\n      \"type\": \"string\",\n      \"nullable\": true\n    },\n    \"members_can_create_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"nullable\": true\n    },\n    \"two_factor_requirement_enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"nullable\": true\n    },\n    \"members_allowed_repository_creation_type\"\
  : {\n      \"type\": \"string\",\n      \"example\": \"all\"\n    },\n    \"members_can_create_public_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"members_can_create_private_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"members_can_create_internal_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"members_can_create_pages\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"members_can_create_public_pages\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"members_can_create_private_pages\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"members_can_fork_private_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"nullable\": true\n    },\n    \"web_commit_signoff_required\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"advanced_security_enabled_for_new_repositories\"\
  : {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Whether GitHub Advanced Security is enabled for new repositories and repositories transferred to this organization.\\n\\nThis field is only visible to organization owners or members of a team with the security manager role.\"\n    },\n    \"dependabot_alerts_enabled_for_new_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Whether GitHub Advanced Security is automatically enabled for new repositories and repositories transferred to\\nthis organization.\\n\\nThis field is only visible to organization owners or members of a team with the security manager role.\"\n    },\n    \"dependabot_security_updates_enabled_for_new_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Whether dependabot security updates are automatically enabled for new repositories and repositories transferred\\nto this organization.\\\
  n\\nThis field is only visible to organization owners or members of a team with the security manager role.\"\n    },\n    \"dependency_graph_enabled_for_new_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Whether dependency graph is automatically enabled for new repositories and repositories transferred to this\\norganization.\\n\\nThis field is only visible to organization owners or members of a team with the security manager role.\"\n    },\n    \"secret_scanning_enabled_for_new_repositories\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Whether secret scanning is automatically enabled for new repositories and repositories transferred to this\\norganization.\\n\\nThis field is only visible to organization owners or members of a team with the security manager role.\"\n    },\n    \"secret_scanning_push_protection_enabled_for_new_repositories\": {\n      \"type\": \"boolean\",\n      \"example\"\
  : false,\n      \"description\": \"Whether secret scanning push protection is automatically enabled for new repositories and repositories\\ntransferred to this organization.\\n\\nThis field is only visible to organization owners or members of a team with the security manager role.\"\n    },\n    \"secret_scanning_push_protection_custom_link_enabled\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Whether a custom link is shown to contributors who are blocked from pushing a secret by push protection.\"\n    },\n    \"secret_scanning_push_protection_custom_link\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/test-org/test-repo/blob/main/README.md\",\n      \"nullable\": true,\n      \"description\": \"An optional URL string to display to contributors who are blocked from pushing a secret.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2008-01-14T04:33:35Z\"\
  \n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\n    \"login\",\n    \"url\",\n    \"id\",\n    \"node_id\",\n    \"repos_url\",\n    \"events_url\",\n    \"hooks_url\",\n    \"issues_url\",\n    \"members_url\",\n    \"public_members_url\",\n    \"avatar_url\",\n    \"description\",\n    \"html_url\",\n    \"has_organization_projects\",\n    \"has_repository_projects\",\n    \"public_repos\",\n    \"public_gists\",\n    \"followers\",\n    \"following\",\n    \"type\",\n    \"created_at\",\n    \"updated_at\",\n    \"archived_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-organization-full-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: organization-full
---
