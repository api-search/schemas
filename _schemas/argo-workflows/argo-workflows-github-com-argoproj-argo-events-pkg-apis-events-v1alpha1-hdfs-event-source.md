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
