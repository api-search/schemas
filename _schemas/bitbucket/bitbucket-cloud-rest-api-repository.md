---
description: A Bitbucket Cloud repository.
layout: schema
name: Repository
properties_list:
- description: The resource type.
  name: type
  type: string
- description: The repository UUID.
  name: uuid
  type: string
- description: The full name of the repository (workspace/repo-slug).
  name: full_name
  type: string
- description: The name of the repository.
  name: name
  type: string
- description: The URL-friendly slug.
  name: slug
  type: string
- description: The repository description.
  name: description
  type: string
- description: Whether the repository is private.
  name: is_private
  type: boolean
- description: Creation timestamp.
  name: created_on
  type: string
- description: Last update timestamp.
  name: updated_on
  type: string
- description: The size of the repository in bytes.
  name: size
  type: integer
- description: The primary programming language.
  name: language
  type: string
- description: ''
  name: has_issues
  type: boolean
- description: ''
  name: has_wiki
  type: boolean
- description: ''
  name: fork_policy
  type: string
- description: ''
  name: scm
  type: string
- description: The project this repository belongs to.
  name: project
  type: object
- description: ''
  name: mainbranch
  type: object
- description: The owner of the repository.
  name: owner
  type: object
provider_name: Bitbucket
provider_slug: bitbucket
schema_file: json-schema/bitbucket-cloud-rest-api-repository-schema.json
slug: bitbucket-cloud-rest-api-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-repository-schema.json\",\n  \"title\": \"Repository\",\n  \"description\": \"A Bitbucket Cloud repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": { \"type\": \"string\", \"description\": \"The resource type.\" },\n    \"uuid\": { \"type\": \"string\", \"description\": \"The repository UUID.\" },\n    \"full_name\": { \"type\": \"string\", \"description\": \"The full name of the repository (workspace/repo-slug).\" },\n    \"name\": { \"type\": \"string\", \"description\": \"The name of the repository.\" },\n    \"slug\": { \"type\": \"string\", \"description\": \"The URL-friendly slug.\" },\n    \"description\": { \"type\": \"string\", \"description\": \"The repository description.\" },\n    \"is_private\": { \"type\": \"boolean\", \"description\": \"Whether\
  \ the repository is private.\" },\n    \"created_on\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Creation timestamp.\" },\n    \"updated_on\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Last update timestamp.\" },\n    \"size\": { \"type\": \"integer\", \"description\": \"The size of the repository in bytes.\" },\n    \"language\": { \"type\": \"string\", \"description\": \"The primary programming language.\" },\n    \"has_issues\": { \"type\": \"boolean\" },\n    \"has_wiki\": { \"type\": \"boolean\" },\n    \"fork_policy\": { \"type\": \"string\", \"enum\": [\"allow_forks\", \"no_public_forks\", \"no_forks\"] },\n    \"scm\": { \"type\": \"string\", \"enum\": [\"git\", \"hg\"] },\n    \"project\": { \"type\": \"object\", \"description\": \"The project this repository belongs to.\" },\n    \"mainbranch\": { \"type\": \"object\", \"properties\": { \"type\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } } },\n    \"owner\"\
  : { \"type\": \"object\", \"description\": \"The owner of the repository.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bitbucket/refs/heads/main/json-schema/bitbucket-cloud-rest-api-repository-schema.json
tags:
- Atlassian
- CI/CD
- Code Collaboration
- Code Review
- DevOps
- Git
- Pull Requests
- Repository Hosting
- Version Control
title: Repository
---
