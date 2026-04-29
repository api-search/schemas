---
description: PodDNSConfig defines the DNS parameters of a pod in addition to those generated from DNSPolicy.
layout: schema
name: io.k8s.api.core.v1.PodDNSConfig
properties_list:
- description: A list of DNS name server IP addresses. This will be appended to the base nameservers generated from DNSPolicy. Duplicated nameservers will be removed.
  name: nameservers
  type: array
- description: A list of DNS resolver options. This will be merged with the base options generated from DNSPolicy. Duplicated entries will be removed. Resolution options given in Options will override those that app
  name: options
  type: array
- description: A list of DNS search domains for host-name lookup. This will be appended to the base search paths generated from DNSPolicy. Duplicated search paths will be removed.
  name: searches
  type: array
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-pod-dns-config-schema.json
slug: argo-workflows-io-k8s-api-core-v1-pod-dns-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-dns-config-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PodDNSConfig\",\n  \"description\": \"PodDNSConfig defines the DNS parameters of a pod in addition to those generated from DNSPolicy.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nameservers\": {\n      \"description\": \"A list of DNS name server IP addresses. This will be appended to the base nameservers generated from DNSPolicy. Duplicated nameservers will be removed.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"options\": {\n      \"description\": \"A list of DNS resolver options. This will be merged with the base options generated from DNSPolicy. Duplicated entries will be removed. Resolution\
  \ options given in Options will override those that appear in the base DNSPolicy.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.PodDNSConfigOption\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"searches\": {\n      \"description\": \"A list of DNS search domains for host-name lookup. This will be appended to the base search paths generated from DNSPolicy. Duplicated search paths will be removed.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-dns-config-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PodDNSConfig
---
