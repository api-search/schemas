---
description: CommitMetadata contains metadata about a commit that is related in some way to another commit.
layout: schema
name: v1alpha1CommitMetadata
properties_list:
- description: Author is the author of the commit, i.e. `git show -s --format=%an <%ae>`. Must be formatted according to RFC 5322 (mail.Address.String()). Comes from the Argocd-reference-commit-author trailer.
  name: author
  type: string
- description: Body is the commit message body minus the subject line, i.e. `git show -s --format=%b`. Comes from the Argocd-reference-commit-body trailer.
  name: body
  type: string
- description: Date is the date of the commit, formatted as by `git show -s --format=%aI` (RFC 3339). It can also be an empty string if the date is unknown. Comes from the Argocd-reference-commit-date trailer.
  name: date
  type: string
- description: RepoURL is the URL of the repository where the commit is located. Comes from the Argocd-reference-commit-repourl trailer. This value is not validated and should not be used to construct UI links unles
  name: repoUrl
  type: string
- description: SHA is the commit hash. Comes from the Argocd-reference-commit-sha trailer.
  name: sha
  type: string
- description: Subject is the commit message subject line, i.e. `git show -s --format=%s`. Comes from the Argocd-reference-commit-subject trailer.
  name: subject
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-commit-metadata-schema.json
slug: argo-cd-v1alpha1-commit-metadata
source_filename: argo-cd-v1alpha1-commit-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-commit-metadata-schema.json\",\n  \"title\": \"v1alpha1CommitMetadata\",\n  \"description\": \"CommitMetadata contains metadata about a commit that is related in some way to another commit.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"author\": {\n      \"description\": \"Author is the author of the commit, i.e. `git show -s --format=%an <%ae>`.\\nMust be formatted according to RFC 5322 (mail.Address.String()).\\nComes from the Argocd-reference-commit-author trailer.\",\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"description\": \"Body is the commit message body minus the subject line, i.e. `git show -s --format=%b`.\\nComes from the Argocd-reference-commit-body trailer.\",\n      \"type\": \"string\"\n    },\n    \"date\": {\n      \"description\": \"Date is the date\
  \ of the commit, formatted as by `git show -s --format=%aI` (RFC 3339).\\nIt can also be an empty string if the date is unknown.\\nComes from the Argocd-reference-commit-date trailer.\",\n      \"type\": \"string\"\n    },\n    \"repoUrl\": {\n      \"description\": \"RepoURL is the URL of the repository where the commit is located.\\nComes from the Argocd-reference-commit-repourl trailer.\\nThis value is not validated and should not be used to construct UI links unless it is properly\\nvalidated and/or sanitized first.\",\n      \"type\": \"string\"\n    },\n    \"sha\": {\n      \"description\": \"SHA is the commit hash.\\nComes from the Argocd-reference-commit-sha trailer.\",\n      \"type\": \"string\"\n    },\n    \"subject\": {\n      \"description\": \"Subject is the commit message subject line, i.e. `git show -s --format=%s`.\\nComes from the Argocd-reference-commit-subject trailer.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-commit-metadata-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1CommitMetadata
---
