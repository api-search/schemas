---
description: CreateOptions may be provided when creating an API object.
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.CreateOptions
properties_list:
- description: ''
  name: dryRun
  type: array
- description: ''
  name: fieldManager
  type: string
- description: ''
  name: fieldValidation
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-create-options-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-create-options
source_filename: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-create-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-create-options-schema.json\",\n  \"title\": \"io.k8s.apimachinery.pkg.apis.meta.v1.CreateOptions\",\n  \"description\": \"CreateOptions may be provided when creating an API object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dryRun\": {\n      \"type\": \"array\",\n      \"title\": \"When present, indicates that modifications should not be\\npersisted. An invalid or unrecognized dryRun directive will\\nresult in an error response and no further processing of the\\nrequest. Valid values are:\\n- All: all dry run stages will be processed\\n+optional\\n+listType=atomic\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"fieldManager\": {\n      \"type\": \"string\",\n      \"title\": \"fieldManager is a name associated\
  \ with the actor or entity\\nthat is making these changes. The value must be less than or\\n128 characters long, and only contain printable characters,\\nas defined by https://golang.org/pkg/unicode/#IsPrint.\\n+optional\"\n    },\n    \"fieldValidation\": {\n      \"type\": \"string\",\n      \"title\": \"fieldValidation instructs the server on how to handle\\nobjects in the request (POST/PUT/PATCH) containing unknown\\nor duplicate fields. Valid values are:\\n- Ignore: This will ignore any unknown fields that are silently\\ndropped from the object, and will ignore all but the last duplicate\\nfield that the decoder encounters. This is the default behavior\\nprior to v1.23.\\n- Warn: This will send a warning via the standard warning response\\nheader for each unknown field that is dropped from the object, and\\nfor each duplicate field that is encountered. The request will\\nstill succeed if there are no other errors, and will only persist\\nthe last of any duplicate fields. This is the\
  \ default in v1.23+\\n- Strict: This will fail the request with a BadRequest error if\\nany unknown fields would be dropped from the object, or if any\\nduplicate fields are present. The error returned from the server\\nwill contain all unknown and duplicate fields encountered.\\n+optional\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-create-options-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.CreateOptions
---
