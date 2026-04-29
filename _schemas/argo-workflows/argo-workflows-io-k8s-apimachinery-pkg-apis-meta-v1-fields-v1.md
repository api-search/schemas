---
description: 'FieldsV1 stores a set of fields in a data structure like a Trie, in JSON format. Each key is either a ''.'' representing the field itself, and will always map to an empty set, or a string representing a sub-field or item. The string will follow one of these four formats: ''f:<name>'', where <name> is the name of a field in a struct, or key in a map ''v:<value>'', where <value> is the exact json formatted value of a list item ''i:<index>'', where <index> is position of a item in a list ''k:<keys>'', where <keys> is a map of a list item''s key fields to their unique values If a key maps to an empty Fields value, the field that key represents is part of the set. The exact format is defined in sigs.k8s.io/structured-merge-diff'
layout: schema
name: io.k8s.apimachinery.pkg.apis.meta.v1.FieldsV1
properties_list: []
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-fields-v1-schema.json
slug: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-fields-v1
source_filename: argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-fields-v1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-fields-v1-schema.json\",\n  \"title\": \"io.k8s.apimachinery.pkg.apis.meta.v1.FieldsV1\",\n  \"description\": \"FieldsV1 stores a set of fields in a data structure like a Trie, in JSON format.\\n\\nEach key is either a '.' representing the field itself, and will always map to an empty set, or a string representing a sub-field or item. The string will follow one of these four formats: 'f:<name>', where <name> is the name of a field in a struct, or key in a map 'v:<value>', where <value> is the exact json formatted value of a list item 'i:<index>', where <index> is position of a item in a list 'k:<keys>', where <keys> is a map of  a list item's key fields to their unique values If a key maps to an empty Fields value, the field that key represents is part\
  \ of the set.\\n\\nThe exact format is defined in sigs.k8s.io/structured-merge-diff\",\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-apimachinery-pkg-apis-meta-v1-fields-v1-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.apimachinery.pkg.apis.meta.v1.FieldsV1
---
