---
description: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HDFSEventSource schema from Argo Workflows API
layout: schema
name: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HDFSEventSource
properties_list:
- description: ''
  name: addresses
  type: array
- description: ''
  name: checkInterval
  type: string
- description: ''
  name: filter
  type: object
- description: HDFSUser is the user to access HDFS file system. It is ignored if either ccache or keytab is used.
  name: hdfsUser
  type: string
- description: KrbCCacheSecret is the secret selector for Kerberos ccache Either ccache or keytab can be set to use Kerberos.
  name: krbCCacheSecret
  type: object
- description: KrbConfig is the configmap selector for Kerberos config as string It must be set if either ccache or keytab is used.
  name: krbConfigConfigMap
  type: object
- description: KrbKeytabSecret is the secret selector for Kerberos keytab Either ccache or keytab can be set to use Kerberos.
  name: krbKeytabSecret
  type: object
- description: KrbRealm is the Kerberos realm used with Kerberos keytab It must be set if keytab is used.
  name: krbRealm
  type: string
- description: KrbServicePrincipalName is the principal name of Kerberos service It must be set if either ccache or keytab is used.
  name: krbServicePrincipalName
  type: string
- description: KrbUsername is the Kerberos username used with Kerberos keytab It must be set if keytab is used.
  name: krbUsername
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: type
  type: string
- description: ''
  name: watchPathConfig
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-hdfs-event-source-schema.json
slug: argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-hdfs-event-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-hdfs-event-source-schema.json\",\n  \"title\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HDFSEventSource\",\n  \"description\": \"github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HDFSEventSource schema from Argo Workflows API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"addresses\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"checkInterval\": {\n      \"type\": \"string\",\n      \"title\": \"CheckInterval is a string that describes an interval duration to check the directory state, e.g. 1s, 30m, 2h... (defaults to 1m)\"\n    },\n    \"filter\": {\n      \"title\": \"Filter\\n+optional\",\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.EventSourceFilter\"\
  \n    },\n    \"hdfsUser\": {\n      \"description\": \"HDFSUser is the user to access HDFS file system.\\nIt is ignored if either ccache or keytab is used.\",\n      \"type\": \"string\"\n    },\n    \"krbCCacheSecret\": {\n      \"description\": \"KrbCCacheSecret is the secret selector for Kerberos ccache\\nEither ccache or keytab can be set to use Kerberos.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"krbConfigConfigMap\": {\n      \"description\": \"KrbConfig is the configmap selector for Kerberos config as string\\nIt must be set if either ccache or keytab is used.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapKeySelector\"\n    },\n    \"krbKeytabSecret\": {\n      \"description\": \"KrbKeytabSecret is the secret selector for Kerberos keytab\\nEither ccache or keytab can be set to use Kerberos.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretKeySelector\"\n    },\n    \"krbRealm\": {\n      \"description\"\
  : \"KrbRealm is the Kerberos realm used with Kerberos keytab\\nIt must be set if keytab is used.\",\n      \"type\": \"string\"\n    },\n    \"krbServicePrincipalName\": {\n      \"description\": \"KrbServicePrincipalName is the principal name of Kerberos service\\nIt must be set if either ccache or keytab is used.\",\n      \"type\": \"string\"\n    },\n    \"krbUsername\": {\n      \"description\": \"KrbUsername is the Kerberos username used with Kerberos keytab\\nIt must be set if keytab is used.\",\n      \"type\": \"string\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"title\": \"Metadata holds the user defined metadata which will passed along the event payload.\\n+optional\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"title\": \"Type of file operations to watch\"\n    },\n    \"watchPathConfig\": {\n      \"$ref\": \"#/definitions/github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.WatchPathConfig\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-github-com-argoproj-argo-events-pkg-apis-events-v1alpha1-hdfs-event-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: github.com.argoproj.argo_events.pkg.apis.events.v1alpha1.HDFSEventSource
---
