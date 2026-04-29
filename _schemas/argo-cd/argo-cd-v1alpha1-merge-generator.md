---
description: 'MergeGenerator merges the output of two or more generators. Where the values for all specified merge keys are equal between two sets of generated parameters, the parameter sets will be merged with the parameters from the latter generator taking precedence. Parameter sets with merge keys not present in the base generator''s params will be ignored. For example, if the first generator produced [{a: ''1'', b: ''2''}, {c: ''1'', d: ''1''}] and the second generator produced [{''a'': ''override''}], the united parameters for merge keys = [''a''] would be [{a: ''override'', b: ''1''}, {c: ''1'', d: ''1''}]. MergeGenerator supports template overriding. If a MergeGenerator is one of multiple top-level generators, its template will be merged with the top-level generator before the parameters are applied.'
layout: schema
name: v1alpha1MergeGenerator
properties_list:
- description: ''
  name: generators
  type: array
- description: ''
  name: mergeKeys
  type: array
- description: ''
  name: template
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-merge-generator-schema.json
slug: argo-cd-v1alpha1-merge-generator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-merge-generator-schema.json\",\n  \"title\": \"v1alpha1MergeGenerator\",\n  \"description\": \"MergeGenerator merges the output of two or more generators. Where the values for all specified merge keys are equal\\nbetween two sets of generated parameters, the parameter sets will be merged with the parameters from the latter\\ngenerator taking precedence. Parameter sets with merge keys not present in the base generator's params will be\\nignored.\\nFor example, if the first generator produced [{a: '1', b: '2'}, {c: '1', d: '1'}] and the second generator produced\\n[{'a': 'override'}], the united parameters for merge keys = ['a'] would be\\n[{a: 'override', b: '1'}, {c: '1', d: '1'}].\\n\\nMergeGenerator supports template overriding. If a MergeGenerator is one of multiple top-level generators, its\\\
  ntemplate will be merged with the top-level generator before the parameters are applied.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"generators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSetNestedGenerator\"\n      }\n    },\n    \"mergeKeys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-merge-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1MergeGenerator
---
