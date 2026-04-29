---
description: RevisionMetadata contains metadata for a specific revision in a Git repository. This field is used by the Source Hydrator feature which may be removed in the future.
layout: schema
name: v1alpha1RevisionMetadata
properties_list:
- description: ''
  name: author
  type: string
- description: ''
  name: date
  type: object
- description: Message contains the message associated with the revision, most likely the commit message.
  name: message
  type: string
- description: References contains references to information that's related to this commit in some way.
  name: references
  type: array
- description: SignatureInfo contains a hint on the signer if the revision was signed with GPG, and signature verification is enabled.
  name: signatureInfo
  type: string
- description: ''
  name: tags
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-revision-metadata-schema.json
slug: argo-cd-v1alpha1-revision-metadata
source_filename: argo-cd-v1alpha1-revision-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-revision-metadata-schema.json\",\n  \"title\": \"v1alpha1RevisionMetadata\",\n  \"description\": \"RevisionMetadata contains metadata for a specific revision in a Git repository. This field is used by the\\nSource Hydrator feature which may be removed in the future.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"author\": {\n      \"type\": \"string\",\n      \"title\": \"who authored this revision,\\ntypically their name and email, e.g. \\\"John Doe <john_doe@my-company.com>\\\",\\nbut might not match this example\"\n    },\n    \"date\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"message\": {\n      \"description\": \"Message contains the message associated with the revision, most likely the commit message.\",\n      \"type\": \"string\"\n    },\n    \"references\":\
  \ {\n      \"description\": \"References contains references to information that's related to this commit in some way.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1RevisionReference\"\n      }\n    },\n    \"signatureInfo\": {\n      \"description\": \"SignatureInfo contains a hint on the signer if the revision was signed with GPG, and signature verification is enabled.\",\n      \"type\": \"string\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"title\": \"Tags specifies any tags currently attached to the revision\\nFloating tags can move from one revision to another\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-revision-metadata-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RevisionMetadata
---
