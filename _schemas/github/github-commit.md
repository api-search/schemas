---
description: A Git commit in a GitHub repository, including metadata about the author, committer, tree, parents, and verification status.
layout: schema
name: GitHub Commit
properties_list:
- description: The SHA-1 hash of the commit.
  name: sha
  type: string
- description: The GraphQL node ID for the commit.
  name: node_id
  type: string
- description: The API URL for the commit.
  name: url
  type: string
- description: The URL of the commit on GitHub.
  name: html_url
  type: string
- description: The API URL for the commit's comments.
  name: comments_url
  type: string
- description: ''
  name: commit
  type: object
- description: The GitHub user who authored the commit.
  name: author
  type: object
- description: The GitHub user who committed the changes.
  name: committer
  type: object
- description: The parent commits of this commit.
  name: parents
  type: array
- description: Statistics about the commit changes.
  name: stats
  type: object
- description: The files changed in the commit.
  name: files
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-commit-schema.json
slug: github-commit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/schemas/github/commit.json\",\n  \"title\": \"GitHub Commit\",\n  \"description\": \"A Git commit in a GitHub repository, including metadata about the author, committer, tree, parents, and verification status.\",\n  \"type\": \"object\",\n  \"required\": [\"sha\", \"commit\"],\n  \"properties\": {\n    \"sha\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[0-9a-f]{40}$\",\n      \"description\": \"The SHA-1 hash of the commit.\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"description\": \"The GraphQL node ID for the commit.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the commit.\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the commit on GitHub.\"\n    },\n    \"comments_url\": {\n     \
  \ \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The API URL for the commit's comments.\"\n    },\n    \"commit\": {\n      \"$ref\": \"#/$defs/GitCommit\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/SimpleUser\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The GitHub user who authored the commit.\"\n    },\n    \"committer\": {\n      \"oneOf\": [\n        { \"$ref\": \"#/$defs/SimpleUser\" },\n        { \"type\": \"null\" }\n      ],\n      \"description\": \"The GitHub user who committed the changes.\"\n    },\n    \"parents\": {\n      \"type\": \"array\",\n      \"description\": \"The parent commits of this commit.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ParentCommit\"\n      }\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Statistics about the commit changes.\",\n      \"properties\": {\n        \"additions\": {\n          \"type\": \"integer\",\n\
  \          \"minimum\": 0,\n          \"description\": \"The number of lines added.\"\n        },\n        \"deletions\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of lines deleted.\"\n        },\n        \"total\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The total number of lines changed.\"\n        }\n      }\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"description\": \"The files changed in the commit.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/CommitFile\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"GitCommit\": {\n      \"type\": \"object\",\n      \"description\": \"The underlying Git commit object data.\",\n      \"required\": [\"message\", \"tree\", \"author\", \"committer\"],\n      \"properties\": {\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"The commit message.\"\n        },\n        \"tree\"\
  : {\n          \"type\": \"object\",\n          \"description\": \"The tree object the commit points to.\",\n          \"properties\": {\n            \"sha\": {\n              \"type\": \"string\",\n              \"pattern\": \"^[0-9a-f]{40}$\",\n              \"description\": \"The SHA of the tree.\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\",\n              \"description\": \"The API URL for the tree.\"\n            }\n          }\n        },\n        \"author\": {\n          \"$ref\": \"#/$defs/GitUser\"\n        },\n        \"committer\": {\n          \"$ref\": \"#/$defs/GitUser\"\n        },\n        \"verification\": {\n          \"$ref\": \"#/$defs/Verification\"\n        },\n        \"comment_count\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of comments on the commit.\"\n        }\n      }\n    },\n    \"GitUser\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"A Git user (author or committer) with name, email, and timestamp.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the Git user.\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The email address of the Git user.\"\n        },\n        \"date\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of the action.\"\n        }\n      }\n    },\n    \"SimpleUser\": {\n      \"type\": \"object\",\n      \"description\": \"A simplified representation of a GitHub user.\",\n      \"required\": [\"login\", \"id\"],\n      \"properties\": {\n        \"login\": {\n          \"type\": \"string\",\n          \"description\": \"The username of the user.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The unique\
  \ identifier for the user.\"\n        },\n        \"node_id\": {\n          \"type\": \"string\",\n          \"description\": \"The GraphQL node ID.\"\n        },\n        \"avatar_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image.\"\n        },\n        \"html_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's GitHub profile.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"User\", \"Organization\", \"Bot\"],\n          \"description\": \"The type of account.\"\n        }\n      }\n    },\n    \"ParentCommit\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a parent commit.\",\n      \"required\": [\"sha\", \"url\"],\n      \"properties\": {\n        \"sha\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9a-f]{40}$\",\n          \"description\":\
  \ \"The SHA of the parent commit.\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The API URL for the parent commit.\"\n        },\n        \"html_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL of the parent commit on GitHub.\"\n        }\n      }\n    },\n    \"CommitFile\": {\n      \"type\": \"object\",\n      \"description\": \"A file changed in a commit.\",\n      \"properties\": {\n        \"sha\": {\n          \"type\": \"string\",\n          \"description\": \"The SHA of the file blob.\"\n        },\n        \"filename\": {\n          \"type\": \"string\",\n          \"description\": \"The path and name of the file.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"added\", \"removed\", \"modified\", \"renamed\", \"copied\", \"changed\", \"unchanged\"],\n          \"description\": \"The status\
  \ of the file change.\"\n        },\n        \"additions\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of lines added.\"\n        },\n        \"deletions\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of lines deleted.\"\n        },\n        \"changes\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The total number of changes.\"\n        },\n        \"patch\": {\n          \"type\": \"string\",\n          \"description\": \"The unified diff patch for the file.\"\n        },\n        \"previous_filename\": {\n          \"type\": \"string\",\n          \"description\": \"The previous filename if the file was renamed.\"\n        }\n      }\n    },\n    \"Verification\": {\n      \"type\": \"object\",\n      \"description\": \"Commit signature verification status.\",\n      \"properties\": {\n        \"verified\": {\n     \
  \     \"type\": \"boolean\",\n          \"description\": \"Whether the signature was verified.\"\n        },\n        \"reason\": {\n          \"type\": \"string\",\n          \"enum\": [\"expired_key\", \"not_signing_key\", \"gpgverify_error\", \"gpgverify_unavailable\", \"unsigned\", \"unknown_signature_type\", \"no_user\", \"unverified_email\", \"bad_email\", \"unknown_key\", \"malformed_signature\", \"invalid\", \"valid\", \"bad_cert\", \"ocsp_pending\"],\n          \"description\": \"The reason for the verification result.\"\n        },\n        \"signature\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The signature that was extracted from the commit.\"\n        },\n        \"payload\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The payload that was signed.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-commit-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: GitHub Commit
---
