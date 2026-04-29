---
description: applicationApplicationManifestQueryWithFilesWrapper schema from Argo CD API
layout: schema
name: applicationApplicationManifestQueryWithFilesWrapper
properties_list:
- description: ''
  name: chunk
  type: object
- description: ''
  name: query
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-application-application-manifest-query-with-files-wrapper-schema.json
slug: argo-cd-application-application-manifest-query-with-files-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-manifest-query-with-files-wrapper-schema.json\",\n  \"title\": \"applicationApplicationManifestQueryWithFilesWrapper\",\n  \"description\": \"applicationApplicationManifestQueryWithFilesWrapper schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chunk\": {\n      \"$ref\": \"#/definitions/applicationFileChunk\"\n    },\n    \"query\": {\n      \"$ref\": \"#/definitions/applicationApplicationManifestQueryWithFiles\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-application-application-manifest-query-with-files-wrapper-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: applicationApplicationManifestQueryWithFilesWrapper
---
