---
description: repository on GitHub.
layout: schema
name: repository
properties_list:
- description: Unique identifier of the repository
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: The name of the repository.
  name: name
  type: string
- description: ''
  name: full_name
  type: string
- description: ''
  name: license
  type: object
- description: ''
  name: forks
  type: integer
- description: ''
  name: permissions
  type: object
- description: ''
  name: owner
  type: object
- description: Whether the repository is private or public.
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
- description: The default branch of the repository.
  name: default_branch
  type: string
- description: ''
  name: open_issues_count
  type: integer
- description: Whether this repository acts as a template that can be used to generate new repositories.
  name: is_template
  type: boolean
- description: ''
  name: topics
  type: array
- description: Whether issues are enabled.
  name: has_issues
  type: boolean
- description: Whether projects are enabled.
  name: has_projects
  type: boolean
- description: Whether the wiki is enabled.
  name: has_wiki
  type: boolean
- description: ''
  name: has_pages
  type: boolean
- description: Whether downloads are enabled.
  name: has_downloads
  type: boolean
- description: Whether discussions are enabled.
  name: has_discussions
  type: boolean
- description: Whether the repository is archived.
  name: archived
  type: boolean
- description: Returns whether or not this repository disabled.
  name: disabled
  type: boolean
- description: 'The repository visibility: public, private, or internal.'
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
- description: Whether to allow rebase merges for pull requests.
  name: allow_rebase_merge
  type: boolean
- description: ''
  name: temp_clone_token
  type: string
- description: Whether to allow squash merges for pull requests.
  name: allow_squash_merge
  type: boolean
- description: Whether to allow Auto-merge to be used on pull requests.
  name: allow_auto_merge
  type: boolean
- description: Whether to delete head branches when pull requests are merged
  name: delete_branch_on_merge
  type: boolean
- description: Whether or not a pull request head branch that is behind its base branch can always be updated even if it is not required to be up to date before merging.
  name: allow_update_branch
  type: boolean
- description: Whether a squash merge commit can use the pull request title as default. **This property has been deprecated. Please use `squash_merge_commit_title` instead.
  name: use_squash_pr_title_as_default
  type: boolean
- description: 'The default value for a squash merge commit title: - `PR_TITLE` - default to the pull request''s title. - `COMMIT_OR_PR_TITLE` - default to the commit''s title (if only one commit) or the pull request''s'
  name: squash_merge_commit_title
  type: string
- description: 'The default value for a squash merge commit message: - `PR_BODY` - default to the pull request''s body. - `COMMIT_MESSAGES` - default to the branch''s commit messages. - `BLANK` - default to a blank com'
  name: squash_merge_commit_message
  type: string
- description: 'The default value for a merge commit title. - `PR_TITLE` - default to the pull request''s title. - `MERGE_MESSAGE` - default to the classic title for a merge message (e.g., Merge pull request #123 from'
  name: merge_commit_title
  type: string
- description: The default value for a merge commit message. - `PR_TITLE` - default to the pull request's title. - `PR_BODY` - default to the pull request's body. - `BLANK` - default to a blank commit message.
  name: merge_commit_message
  type: string
- description: Whether to allow merge commits for pull requests.
  name: allow_merge_commit
  type: boolean
- description: Whether to allow forking this repo
  name: allow_forking
  type: boolean
- description: Whether to require contributors to sign off on web-based commits
  name: web_commit_signoff_required
  type: boolean
- description: ''
  name: open_issues
  type: integer
- description: ''
  name: watchers
  type: integer
- description: ''
  name: master_branch
  type: string
- description: ''
  name: starred_at
  type: string
- description: Whether anonymous git access is enabled for this repository
  name: anonymous_access_enabled
  type: boolean
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-issues-api-repository-schema.json
slug: github-repo-issues-api-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-issues-api-repository-schema.json\",\n  \"title\": \"repository\",\n  \"description\": \"repository on GitHub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Unique identifier of the repository\",\n      \"example\": 42,\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDEwOlJlcG9zaXRvcnkxMjk2MjY5\"\n    },\n    \"name\": {\n      \"description\": \"The name of the repository.\",\n      \"type\": \"string\",\n      \"example\": \"Team Environment\"\n    },\n    \"full_name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat/Hello-World\"\n    },\n    \"license\": {\n      \"$ref\": \"#/components/schemas/nullable-license-simple\"\n    },\n    \"forks\": {\n\
  \      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"permissions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"admin\": {\n          \"type\": \"boolean\"\n        },\n        \"pull\": {\n          \"type\": \"boolean\"\n        },\n        \"triage\": {\n          \"type\": \"boolean\"\n        },\n        \"push\": {\n          \"type\": \"boolean\"\n        },\n        \"maintain\": {\n          \"type\": \"boolean\"\n        }\n      },\n      \"required\": [\n        \"admin\",\n        \"pull\",\n        \"push\"\n      ]\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/simple-user\"\n    },\n    \"private\": {\n      \"description\": \"Whether the repository is private or public.\",\n      \"default\": false,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/octocat/Hello-World\"\n    },\n   \
  \ \"description\": {\n      \"type\": \"string\",\n      \"example\": \"This your first repo!\"\n    },\n    \"fork\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"archive_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/{archive_format}{/ref}\"\n    },\n    \"assignees_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/assignees{/user}\"\n    },\n    \"blobs_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/blobs{/sha}\"\n    },\n    \"branches_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/branches{/branch}\"\n    },\n    \"collaborators_url\": {\n      \"type\": \"string\"\
  ,\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/collaborators{/collaborator}\"\n    },\n    \"comments_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/comments{/number}\"\n    },\n    \"commits_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/commits{/sha}\"\n    },\n    \"compare_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/compare/{base}...{head}\"\n    },\n    \"contents_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/contents/{+path}\"\n    },\n    \"contributors_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/contributors\"\n    },\n    \"deployments_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\"\
  : \"http://api.github.com/repos/octocat/Hello-World/deployments\"\n    },\n    \"downloads_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/downloads\"\n    },\n    \"events_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/events\"\n    },\n    \"forks_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/forks\"\n    },\n    \"git_commits_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/commits{/sha}\"\n    },\n    \"git_refs_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/refs{/sha}\"\n    },\n    \"git_tags_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/git/tags{/sha}\"\
  \n    },\n    \"git_url\": {\n      \"type\": \"string\",\n      \"example\": \"git:github.com/octocat/Hello-World.git\"\n    },\n    \"issue_comment_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/issues/comments{/number}\"\n    },\n    \"issue_events_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/issues/events{/number}\"\n    },\n    \"issues_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/issues{/number}\"\n    },\n    \"keys_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/keys{/key_id}\"\n    },\n    \"labels_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/labels{/name}\"\n    },\n    \"languages_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/languages\"\
  \n    },\n    \"merges_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/merges\"\n    },\n    \"milestones_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/milestones{/number}\"\n    },\n    \"notifications_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/notifications{?since,all,participating}\"\n    },\n    \"pulls_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/pulls{/number}\"\n    },\n    \"releases_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/releases{/id}\"\n    },\n    \"ssh_url\": {\n      \"type\": \"string\",\n      \"example\": \"git@github.com:octocat/Hello-World.git\"\n    },\n    \"stargazers_url\": {\n      \"type\": \"string\",\n      \"format\":\
  \ \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/stargazers\"\n    },\n    \"statuses_url\": {\n      \"type\": \"string\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/statuses/{sha}\"\n    },\n    \"subscribers_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/subscribers\"\n    },\n    \"subscription_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/subscription\"\n    },\n    \"tags_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/tags\"\n    },\n    \"teams_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/teams\"\n    },\n    \"trees_url\": {\n      \"type\": \"string\",\n      \"example\"\
  : \"http://api.github.com/repos/octocat/Hello-World/git/trees{/sha}\"\n    },\n    \"clone_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://github.com/octocat/Hello-World.git\"\n    },\n    \"mirror_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"git:git.example.com/octocat/Hello-World\"\n    },\n    \"hooks_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"http://api.github.com/repos/octocat/Hello-World/hooks\"\n    },\n    \"svn_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://svn.github.com/octocat/Hello-World\"\n    },\n    \"homepage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com\"\n    },\n    \"language\": {\n      \"type\": \"string\"\n    },\n    \"forks_count\": {\n      \"type\": \"integer\",\n      \"example\": 9\n    },\n    \"stargazers_count\": {\n      \"type\": \"integer\"\
  ,\n      \"example\": 80\n    },\n    \"watchers_count\": {\n      \"type\": \"integer\",\n      \"example\": 80\n    },\n    \"size\": {\n      \"description\": \"The size of the repository, in kilobytes. Size is calculated hourly. When a repository is initially created, the size is 0.\",\n      \"type\": \"integer\",\n      \"example\": 108\n    },\n    \"default_branch\": {\n      \"description\": \"The default branch of the repository.\",\n      \"type\": \"string\",\n      \"example\": \"master\"\n    },\n    \"open_issues_count\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    },\n    \"is_template\": {\n      \"description\": \"Whether this repository acts as a template that can be used to generate new repositories.\",\n      \"default\": false,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"has_issues\": {\n      \"description\": \"\
  Whether issues are enabled.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"has_projects\": {\n      \"description\": \"Whether projects are enabled.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"has_wiki\": {\n      \"description\": \"Whether the wiki is enabled.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"has_pages\": {\n      \"type\": \"boolean\"\n    },\n    \"has_downloads\": {\n      \"description\": \"Whether downloads are enabled.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true,\n      \"deprecated\": true\n    },\n    \"has_discussions\": {\n      \"description\": \"Whether discussions are enabled.\",\n      \"default\": false,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"archived\": {\n      \"description\": \"Whether the repository is archived.\",\n      \"\
  default\": false,\n      \"type\": \"boolean\"\n    },\n    \"disabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Returns whether or not this repository disabled.\"\n    },\n    \"visibility\": {\n      \"description\": \"The repository visibility: public, private, or internal.\",\n      \"default\": \"public\",\n      \"type\": \"string\"\n    },\n    \"pushed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-01-26T19:06:43Z\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-01-26T19:01:12Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-01-26T19:14:43Z\"\n    },\n    \"allow_rebase_merge\": {\n      \"description\": \"Whether to allow rebase merges for pull requests.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"temp_clone_token\"\
  : {\n      \"type\": \"string\"\n    },\n    \"allow_squash_merge\": {\n      \"description\": \"Whether to allow squash merges for pull requests.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"allow_auto_merge\": {\n      \"description\": \"Whether to allow Auto-merge to be used on pull requests.\",\n      \"default\": false,\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"delete_branch_on_merge\": {\n      \"description\": \"Whether to delete head branches when pull requests are merged\",\n      \"default\": false,\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"allow_update_branch\": {\n      \"description\": \"Whether or not a pull request head branch that is behind its base branch can always be updated even if it is not required to be up to date before merging.\",\n      \"default\": false,\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"use_squash_pr_title_as_default\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether a squash merge commit can use the pull request title as default. **This property has been deprecated. Please use `squash_merge_commit_title` instead.\",\n      \"default\": false,\n      \"deprecated\": true\n    },\n    \"squash_merge_commit_title\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PR_TITLE\",\n        \"COMMIT_OR_PR_TITLE\"\n      ],\n      \"description\": \"The default value for a squash merge commit title:\\n\\n- `PR_TITLE` - default to the pull request's title.\\n- `COMMIT_OR_PR_TITLE` - default to the commit's title (if only one commit) or the pull request's title (when more than one commit).\"\n    },\n    \"squash_merge_commit_message\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PR_BODY\",\n        \"COMMIT_MESSAGES\",\n        \"BLANK\"\n      ],\n      \"description\": \"The default value for a squash merge commit message:\\n\\n- `PR_BODY` - default to the pull\
  \ request's body.\\n- `COMMIT_MESSAGES` - default to the branch's commit messages.\\n- `BLANK` - default to a blank commit message.\"\n    },\n    \"merge_commit_title\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PR_TITLE\",\n        \"MERGE_MESSAGE\"\n      ],\n      \"description\": \"The default value for a merge commit title.\\n\\n- `PR_TITLE` - default to the pull request's title.\\n- `MERGE_MESSAGE` - default to the classic title for a merge message (e.g., Merge pull request #123 from branch-name).\"\n    },\n    \"merge_commit_message\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PR_BODY\",\n        \"PR_TITLE\",\n        \"BLANK\"\n      ],\n      \"description\": \"The default value for a merge commit message.\\n\\n- `PR_TITLE` - default to the pull request's title.\\n- `PR_BODY` - default to the pull request's body.\\n- `BLANK` - default to a blank commit message.\"\n    },\n    \"allow_merge_commit\": {\n      \"description\": \"Whether to\
  \ allow merge commits for pull requests.\",\n      \"default\": true,\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"allow_forking\": {\n      \"description\": \"Whether to allow forking this repo\",\n      \"type\": \"boolean\"\n    },\n    \"web_commit_signoff_required\": {\n      \"description\": \"Whether to require contributors to sign off on web-based commits\",\n      \"default\": false,\n      \"type\": \"boolean\"\n    },\n    \"open_issues\": {\n      \"type\": \"integer\"\n    },\n    \"watchers\": {\n      \"type\": \"integer\"\n    },\n    \"master_branch\": {\n      \"type\": \"string\"\n    },\n    \"starred_at\": {\n      \"type\": \"string\",\n      \"example\": \"\\\"2020-07-09T00:17:42Z\\\"\"\n    },\n    \"anonymous_access_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether anonymous git access is enabled for this repository\"\n    }\n  },\n  \"required\": [\n    \"archive_url\",\n    \"assignees_url\",\n    \"blobs_url\"\
  ,\n    \"branches_url\",\n    \"collaborators_url\",\n    \"comments_url\",\n    \"commits_url\",\n    \"compare_url\",\n    \"contents_url\",\n    \"contributors_url\",\n    \"deployments_url\",\n    \"description\",\n    \"downloads_url\",\n    \"events_url\",\n    \"fork\",\n    \"forks_url\",\n    \"full_name\",\n    \"git_commits_url\",\n    \"git_refs_url\",\n    \"git_tags_url\",\n    \"hooks_url\",\n    \"html_url\",\n    \"id\",\n    \"node_id\",\n    \"issue_comment_url\",\n    \"issue_events_url\",\n    \"issues_url\",\n    \"keys_url\",\n    \"labels_url\",\n    \"languages_url\",\n    \"merges_url\",\n    \"milestones_url\",\n    \"name\",\n    \"notifications_url\",\n    \"owner\",\n    \"private\",\n    \"pulls_url\",\n    \"releases_url\",\n    \"stargazers_url\",\n    \"statuses_url\",\n    \"subscribers_url\",\n    \"subscription_url\",\n    \"tags_url\",\n    \"teams_url\",\n    \"trees_url\",\n    \"url\",\n    \"clone_url\",\n    \"default_branch\",\n    \"forks\"\
  ,\n    \"forks_count\",\n    \"git_url\",\n    \"has_downloads\",\n    \"has_issues\",\n    \"has_projects\",\n    \"has_wiki\",\n    \"has_pages\",\n    \"homepage\",\n    \"language\",\n    \"archived\",\n    \"disabled\",\n    \"mirror_url\",\n    \"open_issues\",\n    \"open_issues_count\",\n    \"license\",\n    \"pushed_at\",\n    \"size\",\n    \"ssh_url\",\n    \"stargazers_count\",\n    \"svn_url\",\n    \"watchers\",\n    \"watchers_count\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-issues-api-repository-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: repository
---
