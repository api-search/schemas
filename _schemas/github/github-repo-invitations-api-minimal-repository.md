---
description: Minimal Repository
layout: schema
name: minimal-repository
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: full_name
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: private
  type: boolean
- description: ''
  name: html_url
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: fork
  type: boolean
- description: ''
  name: url
  type: string
- description: ''
  name: archive_url
  type: string
- description: ''
  name: assignees_url
  type: string
- description: ''
  name: blobs_url
  type: string
- description: ''
  name: branches_url
  type: string
- description: ''
  name: collaborators_url
  type: string
- description: ''
  name: comments_url
  type: string
- description: ''
  name: commits_url
  type: string
- description: ''
  name: compare_url
  type: string
- description: ''
  name: contents_url
  type: string
- description: ''
  name: contributors_url
  type: string
- description: ''
  name: deployments_url
  type: string
- description: ''
  name: downloads_url
  type: string
- description: ''
  name: events_url
  type: string
- description: ''
  name: forks_url
  type: string
- description: ''
  name: git_commits_url
  type: string
- description: ''
  name: git_refs_url
  type: string
- description: ''
  name: git_tags_url
  type: string
- description: ''
  name: git_url
  type: string
- description: ''
  name: issue_comment_url
  type: string
- description: ''
  name: issue_events_url
  type: string
- description: ''
  name: issues_url
  type: string
- description: ''
  name: keys_url
  type: string
- description: ''
  name: labels_url
  type: string
- description: ''
  name: languages_url
  type: string
- description: ''
  name: merges_url
  type: string
- description: ''
  name: milestones_url
  type: string
- description: ''
  name: notifications_url
  type: string
- description: ''
  name: pulls_url
  type: string
- description: ''
  name: releases_url
  type: string
- description: ''
  name: ssh_url
  type: string
- description: ''
  name: stargazers_url
  type: string
- description: ''
  name: statuses_url
  type: string
- description: ''
  name: subscribers_url
  type: string
- description: ''
  name: subscription_url
  type: string
- description: ''
  name: tags_url
  type: string
- description: ''
  name: teams_url
  type: string
- description: ''
  name: trees_url
  type: string
- description: ''
  name: clone_url
  type: string
- description: ''
  name: mirror_url
  type: string
- description: ''
  name: hooks_url
  type: string
- description: ''
  name: svn_url
  type: string
- description: ''
  name: homepage
  type: string
- description: ''
  name: language
  type: string
- description: ''
  name: forks_count
  type: integer
- description: ''
  name: stargazers_count
  type: integer
- description: ''
  name: watchers_count
  type: integer
- description: The size of the repository, in kilobytes. Size is calculated hourly. When a repository is initially created, the size is 0.
  name: size
  type: integer
- description: ''
  name: default_branch
  type: string
- description: ''
  name: open_issues_count
  type: integer
- description: ''
  name: is_template
  type: boolean
- description: ''
  name: topics
  type: array
- description: ''
  name: has_issues
  type: boolean
- description: ''
  name: has_projects
  type: boolean
- description: ''
  name: has_wiki
  type: boolean
- description: ''
  name: has_pages
  type: boolean
- description: ''
  name: has_downloads
  type: boolean
- description: ''
  name: has_discussions
  type: boolean
- description: ''
  name: archived
  type: boolean
- description: ''
  name: disabled
  type: boolean
- description: ''
  name: visibility
  type: string
- description: ''
  name: pushed_at
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: permissions
  type: object
- description: ''
  name: role_name
  type: string
- description: ''
  name: temp_clone_token
  type: string
- description: ''
  name: delete_branch_on_merge
  type: boolean
- description: ''
  name: subscribers_count
  type: integer
- description: ''
  name: network_count
  type: integer
- description: ''
  name: code_of_conduct
  type: object
- description: ''
  name: license
  type: object
- description: ''
  name: forks
  type: integer
- description: ''
  name: open_issues
  type: integer
- description: ''
  name: watchers
  type: integer
- description: ''
  name: allow_forking
  type: boolean
- description: ''
  name: web_commit_signoff_required
  type: boolean
- description: ''
  name: security_and_analysis
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-invitations-api-minimal-repository-schema.json
slug: github-repo-invitations-api-minimal-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-invitations-api-minimal-repository-schema.json\",\n  \"title\": \"minimal-repository\",\n  \"description\": \"Minimal Repository\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"example\": 1296269\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDEwOlJlcG9zaXRvcnkxMjk2MjY5\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Hello-World\"\n    },\n    \"full_name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat/Hello-World\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/simple-user\"\n    },\n    \"private\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"uri\",\n      \"example\": \"https://github.com/octocat/Hello-World\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"example\": \"This your first repo!\"\n    },\n    \"fork\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"archive_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/{archive_format}{/ref}\"\n    },\n    \"assignees_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/assignees{/user}\"\n    },\n    \"blobs_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/blobs{/sha}\"\n    },\n    \"branches_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/branches{/branch}\"\
  \n    },\n    \"collaborators_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/collaborators{/collaborator}\"\n    },\n    \"comments_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/comments{/number}\"\n    },\n    \"commits_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/commits{/sha}\"\n    },\n    \"compare_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/compare/{base}...{head}\"\n    },\n    \"contents_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/contents/{+path}\"\n    },\n    \"contributors_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/contributors\"\n    },\n    \"deployments_url\": {\n      \"\
  type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/deployments\"\n    },\n    \"downloads_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/downloads\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/events\"\n    },\n    \"forks_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/forks\"\n    },\n    \"git_commits_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/commits{/sha}\"\n    },\n    \"git_refs_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/refs{/sha}\"\n    },\n    \"git_tags_url\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/tags{/sha}\"\n    },\n    \"git_url\": {\n      \"type\": \"string\"\n    },\n    \"issue_comment_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/issues/comments{/number}\"\n    },\n    \"issue_events_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/issues/events{/number}\"\n    },\n    \"issues_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/issues{/number}\"\n    },\n    \"keys_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/keys{/key_id}\"\n    },\n    \"labels_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/labels{/name}\"\n    },\n    \"languages_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n\
  \      \"example\": \"http://api.github.com/repos/octocat/Hello-World/languages\"\n    },\n    \"merges_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/merges\"\n    },\n    \"milestones_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/milestones{/number}\"\n    },\n    \"notifications_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/notifications{?since,all,participating}\"\n    },\n    \"pulls_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/pulls{/number}\"\n    },\n    \"releases_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/releases{/id}\"\n    },\n    \"ssh_url\": {\n      \"type\": \"string\"\n    },\n    \"stargazers_url\": {\n      \"type\": \"string\",\n\
  \      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/stargazers\"\n    },\n    \"statuses_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/statuses/{sha}\"\n    },\n    \"subscribers_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/subscribers\"\n    },\n    \"subscription_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/subscription\"\n    },\n    \"tags_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/tags\"\n    },\n    \"teams_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/teams\"\n    },\n    \"trees_url\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/trees{/sha}\"\n    },\n    \"clone_url\": {\n      \"type\": \"string\"\n    },\n    \"mirror_url\": {\n      \"type\": \"string\"\n    },\n    \"hooks_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/hooks\"\n    },\n    \"svn_url\": {\n      \"type\": \"string\"\n    },\n    \"homepage\": {\n      \"type\": \"string\"\n    },\n    \"language\": {\n      \"type\": \"string\"\n    },\n    \"forks_count\": {\n      \"type\": \"integer\"\n    },\n    \"stargazers_count\": {\n      \"type\": \"integer\"\n    },\n    \"watchers_count\": {\n      \"type\": \"integer\"\n    },\n    \"size\": {\n      \"description\": \"The size of the repository, in kilobytes. Size is calculated hourly. When a repository is initially created, the size is 0.\",\n      \"type\": \"integer\"\n    },\n    \"default_branch\": {\n      \"type\": \"string\"\
  \n    },\n    \"open_issues_count\": {\n      \"type\": \"integer\"\n    },\n    \"is_template\": {\n      \"type\": \"boolean\"\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"has_issues\": {\n      \"type\": \"boolean\"\n    },\n    \"has_projects\": {\n      \"type\": \"boolean\"\n    },\n    \"has_wiki\": {\n      \"type\": \"boolean\"\n    },\n    \"has_pages\": {\n      \"type\": \"boolean\"\n    },\n    \"has_downloads\": {\n      \"type\": \"boolean\"\n    },\n    \"has_discussions\": {\n      \"type\": \"boolean\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"visibility\": {\n      \"type\": \"string\"\n    },\n    \"pushed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-01-26T19:06:43Z\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"example\": \"2011-01-26T19:01:12Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-01-26T19:14:43Z\"\n    },\n    \"permissions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"admin\": {\n          \"type\": \"boolean\"\n        },\n        \"maintain\": {\n          \"type\": \"boolean\"\n        },\n        \"push\": {\n          \"type\": \"boolean\"\n        },\n        \"triage\": {\n          \"type\": \"boolean\"\n        },\n        \"pull\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"role_name\": {\n      \"type\": \"string\",\n      \"example\": \"admin\"\n    },\n    \"temp_clone_token\": {\n      \"type\": \"string\"\n    },\n    \"delete_branch_on_merge\": {\n      \"type\": \"boolean\"\n    },\n    \"subscribers_count\": {\n      \"type\": \"integer\"\n    },\n    \"network_count\": {\n      \"type\": \"integer\"\n    },\n  \
  \  \"code_of_conduct\": {\n      \"$ref\": \"#/components/schemas/code-of-conduct\"\n    },\n    \"license\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"key\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"spdx_id\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        },\n        \"node_id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"forks\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"open_issues\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"watchers\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"allow_forking\": {\n      \"type\": \"boolean\"\n    },\n    \"web_commit_signoff_required\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"security_and_analysis\": {\n      \"$ref\": \"#/components/schemas/security-and-analysis\"\
  \n    }\n  },\n  \"required\": [\n    \"archive_url\",\n    \"assignees_url\",\n    \"blobs_url\",\n    \"branches_url\",\n    \"collaborators_url\",\n    \"comments_url\",\n    \"commits_url\",\n    \"compare_url\",\n    \"contents_url\",\n    \"contributors_url\",\n    \"deployments_url\",\n    \"description\",\n    \"downloads_url\",\n    \"events_url\",\n    \"fork\",\n    \"forks_url\",\n    \"full_name\",\n    \"git_commits_url\",\n    \"git_refs_url\",\n    \"git_tags_url\",\n    \"hooks_url\",\n    \"html_url\",\n    \"id\",\n    \"node_id\",\n    \"issue_comment_url\",\n    \"issue_events_url\",\n    \"issues_url\",\n    \"keys_url\",\n    \"labels_url\",\n    \"languages_url\",\n    \"merges_url\",\n    \"milestones_url\",\n    \"name\",\n    \"notifications_url\",\n    \"owner\",\n    \"private\",\n    \"pulls_url\",\n    \"releases_url\",\n    \"stargazers_url\",\n    \"statuses_url\",\n    \"subscribers_url\",\n    \"subscription_url\",\n    \"tags_url\",\n    \"teams_url\"\
  ,\n    \"trees_url\",\n    \"url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-invitations-api-minimal-repository-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: minimal-repository
---
