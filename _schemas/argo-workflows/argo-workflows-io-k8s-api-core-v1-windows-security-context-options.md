---
description: WindowsSecurityContextOptions contain Windows-specific options and credentials.
layout: schema
name: io.k8s.api.core.v1.WindowsSecurityContextOptions
properties_list:
- description: GMSACredentialSpec is where the GMSA admission webhook (https://github.com/kubernetes-sigs/windows-gmsa) inlines the contents of the GMSA credential spec named by the GMSACredentialSpecName field.
  name: gmsaCredentialSpec
  type: string
- description: GMSACredentialSpecName is the name of the GMSA credential spec to use.
  name: gmsaCredentialSpecName
  type: string
- description: HostProcess determines if a container should be run as a 'Host Process' container. All of a Pod's containers must have the same effective HostProcess value (it is not allowed to have a mix of HostProc
  name: hostProcess
  type: boolean
- description: The UserName in Windows to run the entrypoint of the container process. Defaults to the user specified in image metadata if unspecified. May also be set in PodSecurityContext. If set in both SecurityC
  name: runAsUserName
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-windows-security-context-options-schema.json
slug: argo-workflows-io-k8s-api-core-v1-windows-security-context-options
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.WindowsSecurityContextOptions
---
