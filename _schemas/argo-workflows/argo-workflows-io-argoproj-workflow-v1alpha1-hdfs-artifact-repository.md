---
description: HDFSArtifactRepository defines the controller configuration for an HDFS artifact repository
layout: schema
name: io.argoproj.workflow.v1alpha1.HDFSArtifactRepository
properties_list:
- description: Addresses is accessible addresses of HDFS name nodes
  name: addresses
  type: array
- description: DataTransferProtection is the protection level for HDFS data transfer. It corresponds to the dfs.data.transfer.protection configuration in HDFS.
  name: dataTransferProtection
  type: string
- description: Force copies a file forcibly even if it exists
  name: force
  type: boolean
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
- description: PathFormat is defines the format of path to store a file. Can reference workflow variables
  name: pathFormat
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-argoproj-workflow-v1alpha1-hdfs-artifact-repository-schema.json
slug: argo-workflows-io-argoproj-workflow-v1alpha1-hdfs-artifact-repository
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.argoproj.workflow.v1alpha1.HDFSArtifactRepository
---
