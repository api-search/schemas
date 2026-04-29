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
source_filename: argo-workflows-io-k8s-api-core-v1-windows-security-context-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-windows-security-context-options-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.WindowsSecurityContextOptions\",\n  \"description\": \"WindowsSecurityContextOptions contain Windows-specific options and credentials.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gmsaCredentialSpec\": {\n      \"description\": \"GMSACredentialSpec is where the GMSA admission webhook (https://github.com/kubernetes-sigs/windows-gmsa) inlines the contents of the GMSA credential spec named by the GMSACredentialSpecName field.\",\n      \"type\": \"string\"\n    },\n    \"gmsaCredentialSpecName\": {\n      \"description\": \"GMSACredentialSpecName is the name of the GMSA credential spec to use.\",\n      \"type\": \"string\"\n    },\n    \"hostProcess\": {\n      \"description\": \"\
  HostProcess determines if a container should be run as a 'Host Process' container. All of a Pod's containers must have the same effective HostProcess value (it is not allowed to have a mix of HostProcess containers and non-HostProcess containers). In addition, if HostProcess is true then HostNetwork must also be set to true.\",\n      \"type\": \"boolean\"\n    },\n    \"runAsUserName\": {\n      \"description\": \"The UserName in Windows to run the entrypoint of the container process. Defaults to the user specified in image metadata if unspecified. May also be set in PodSecurityContext. If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-windows-security-context-options-schema.json
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
