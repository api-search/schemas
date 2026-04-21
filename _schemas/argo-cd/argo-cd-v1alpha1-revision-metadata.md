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
