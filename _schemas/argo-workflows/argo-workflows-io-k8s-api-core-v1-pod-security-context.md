---
description: PodSecurityContext holds pod-level security attributes and common container settings. Some fields are also present in container.securityContext. Field values of container.securityContext take precedence over field values of PodSecurityContext.
layout: schema
name: io.k8s.api.core.v1.PodSecurityContext
properties_list:
- description: appArmorProfile is the AppArmor options to use by the containers in this pod. Note that this field cannot be set when spec.os.name is windows.
  name: appArmorProfile
  type: object
- description: 'A special supplemental group that applies to all containers in a pod. Some volume types allow the Kubelet to change the ownership of that volume to be owned by the pod: 1. The owning GID will be the F'
  name: fsGroup
  type: integer
- description: fsGroupChangePolicy defines behavior of changing ownership and permission of the volume before being exposed inside Pod. This field will only apply to volume types which support fsGroup based ownershi
  name: fsGroupChangePolicy
  type: string
- description: The GID to run the entrypoint of the container process. Uses runtime default if unset. May also be set in SecurityContext. If set in both SecurityContext and PodSecurityContext, the value specified in
  name: runAsGroup
  type: integer
- description: Indicates that the container must run as a non-root user. If true, the Kubelet will validate the image at runtime to ensure that it does not run as UID 0 (root) and fail to start the container if it d
  name: runAsNonRoot
  type: boolean
- description: The UID to run the entrypoint of the container process. Defaults to user specified in image metadata if unspecified. May also be set in SecurityContext. If set in both SecurityContext and PodSecurityC
  name: runAsUser
  type: integer
- description: seLinuxChangePolicy defines how the container's SELinux label is applied to all volumes used by the Pod. It has no effect on nodes that do not support SELinux or to volumes does not support SELinux. V
  name: seLinuxChangePolicy
  type: string
- description: The SELinux context to be applied to all containers. If unspecified, the container runtime will allocate a random SELinux context for each container. May also be set in SecurityContext. If set in both
  name: seLinuxOptions
  type: object
- description: The seccomp options to use by the containers in this pod. Note that this field cannot be set when spec.os.name is windows.
  name: seccompProfile
  type: object
- description: A list of groups applied to the first process run in each container, in addition to the container's primary GID and fsGroup (if specified). If the SupplementalGroupsPolicy feature is enabled, the supp
  name: supplementalGroups
  type: array
- description: Defines how supplemental groups of the first container processes are calculated. Valid values are "Merge" and "Strict". If not specified, "Merge" is used. (Alpha) Using the field requires the Suppleme
  name: supplementalGroupsPolicy
  type: string
- description: Sysctls hold a list of namespaced sysctls used for the pod. Pods with unsupported sysctls (by the container runtime) might fail to launch. Note that this field cannot be set when spec.os.name is windo
  name: sysctls
  type: array
- description: The Windows specific settings applied to all containers. If unspecified, the options within a container's SecurityContext will be used. If set in both SecurityContext and PodSecurityContext, the value
  name: windowsOptions
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-pod-security-context-schema.json
slug: argo-workflows-io-k8s-api-core-v1-pod-security-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-security-context-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.PodSecurityContext\",\n  \"description\": \"PodSecurityContext holds pod-level security attributes and common container settings. Some fields are also present in container.securityContext.  Field values of container.securityContext take precedence over field values of PodSecurityContext.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appArmorProfile\": {\n      \"description\": \"appArmorProfile is the AppArmor options to use by the containers in this pod. Note that this field cannot be set when spec.os.name is windows.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.AppArmorProfile\"\n    },\n    \"fsGroup\": {\n      \"description\": \"A special supplemental group that applies to all\
  \ containers in a pod. Some volume types allow the Kubelet to change the ownership of that volume to be owned by the pod:\\n\\n1. The owning GID will be the FSGroup 2. The setgid bit is set (new files created in the volume will be owned by FSGroup) 3. The permission bits are OR'd with rw-rw----\\n\\nIf unset, the Kubelet will not modify the ownership and permissions of any volume. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"integer\"\n    },\n    \"fsGroupChangePolicy\": {\n      \"description\": \"fsGroupChangePolicy defines behavior of changing ownership and permission of the volume before being exposed inside Pod. This field will only apply to volume types which support fsGroup based ownership(and permissions). It will have no effect on ephemeral volume types such as: secret, configmaps and emptydir. Valid values are \\\"OnRootMismatch\\\" and \\\"Always\\\". If not specified, \\\"Always\\\" is used. Note that this field cannot be set when\
  \ spec.os.name is windows.\",\n      \"type\": \"string\"\n    },\n    \"runAsGroup\": {\n      \"description\": \"The GID to run the entrypoint of the container process. Uses runtime default if unset. May also be set in SecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence for that container. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"integer\"\n    },\n    \"runAsNonRoot\": {\n      \"description\": \"Indicates that the container must run as a non-root user. If true, the Kubelet will validate the image at runtime to ensure that it does not run as UID 0 (root) and fail to start the container if it does. If unset or false, no such validation will be performed. May also be set in SecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence.\",\n      \"type\": \"boolean\"\n    },\n    \"runAsUser\": {\n\
  \      \"description\": \"The UID to run the entrypoint of the container process. Defaults to user specified in image metadata if unspecified. May also be set in SecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence for that container. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"integer\"\n    },\n    \"seLinuxChangePolicy\": {\n      \"description\": \"seLinuxChangePolicy defines how the container's SELinux label is applied to all volumes used by the Pod. It has no effect on nodes that do not support SELinux or to volumes does not support SELinux. Valid values are \\\"MountOption\\\" and \\\"Recursive\\\".\\n\\n\\\"Recursive\\\" means relabeling of all files on all Pod volumes by the container runtime. This may be slow for large volumes, but allows mixing privileged and unprivileged Pods sharing the same volume on the same node.\\n\\n\\\"MountOption\\\" mounts all eligible\
  \ Pod volumes with `-o context` mount option. This requires all Pods that share the same volume to use the same SELinux label. It is not possible to share the same volume among privileged and unprivileged Pods. Eligible volumes are in-tree FibreChannel and iSCSI volumes, and all CSI volumes whose CSI driver announces SELinux support by setting spec.seLinuxMount: true in their CSIDriver instance. Other volumes are always re-labelled recursively. \\\"MountOption\\\" value is allowed only when SELinuxMount feature gate is enabled.\\n\\nIf not specified and SELinuxMount feature gate is enabled, \\\"MountOption\\\" is used. If not specified and SELinuxMount feature gate is disabled, \\\"MountOption\\\" is used for ReadWriteOncePod volumes and \\\"Recursive\\\" for all other volumes.\\n\\nThis field affects only Pods that have SELinux label set, either in PodSecurityContext or in SecurityContext of all containers.\\n\\nAll Pods that use the same volume should use the same seLinuxChangePolicy,\
  \ otherwise some pods can get stuck in ContainerCreating state. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"string\"\n    },\n    \"seLinuxOptions\": {\n      \"description\": \"The SELinux context to be applied to all containers. If unspecified, the container runtime will allocate a random SELinux context for each container.  May also be set in SecurityContext.  If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence for that container. Note that this field cannot be set when spec.os.name is windows.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SELinuxOptions\"\n    },\n    \"seccompProfile\": {\n      \"description\": \"The seccomp options to use by the containers in this pod. Note that this field cannot be set when spec.os.name is windows.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SeccompProfile\"\n    },\n    \"supplementalGroups\": {\n      \"description\": \"A\
  \ list of groups applied to the first process run in each container, in addition to the container's primary GID and fsGroup (if specified).  If the SupplementalGroupsPolicy feature is enabled, the supplementalGroupsPolicy field determines whether these are in addition to or instead of any group memberships defined in the container image. If unspecified, no additional groups are added, though group memberships defined in the container image may still be used, depending on the supplementalGroupsPolicy field. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\",\n        \"format\": \"int64\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"supplementalGroupsPolicy\": {\n      \"description\": \"Defines how supplemental groups of the first container processes are calculated. Valid values are \\\"Merge\\\" and \\\"Strict\\\". If not specified, \\\"Merge\\\" is used. (Alpha) Using\
  \ the field requires the SupplementalGroupsPolicy feature gate to be enabled and the container runtime must implement support for this feature. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"string\"\n    },\n    \"sysctls\": {\n      \"description\": \"Sysctls hold a list of namespaced sysctls used for the pod. Pods with unsupported sysctls (by the container runtime) might fail to launch. Note that this field cannot be set when spec.os.name is windows.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/io.k8s.api.core.v1.Sysctl\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"windowsOptions\": {\n      \"description\": \"The Windows specific settings applied to all containers. If unspecified, the options within a container's SecurityContext will be used. If set in both SecurityContext and PodSecurityContext, the value specified in SecurityContext takes precedence. Note that this field cannot\
  \ be set when spec.os.name is linux.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.WindowsSecurityContextOptions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-pod-security-context-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.PodSecurityContext
---
