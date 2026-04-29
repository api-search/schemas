---
description: Represents an ISCSI disk. ISCSI volumes can only be mounted as read/write once. ISCSI volumes support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.ISCSIVolumeSource
properties_list:
- description: chapAuthDiscovery defines whether support iSCSI Discovery CHAP authentication
  name: chapAuthDiscovery
  type: boolean
- description: chapAuthSession defines whether support iSCSI Session CHAP authentication
  name: chapAuthSession
  type: boolean
- description: 'fsType is the filesystem type of the volume that you want to mount. Tip: Ensure that the filesystem type is supported by the host operating system. Examples: "ext4", "xfs", "ntfs". Implicitly inferred'
  name: fsType
  type: string
- description: initiatorName is the custom iSCSI Initiator Name. If initiatorName is specified with iscsiInterface simultaneously, new iSCSI interface <target portal>:<volume name> will be created for the connection
  name: initiatorName
  type: string
- description: iqn is the target iSCSI Qualified Name.
  name: iqn
  type: string
- description: iscsiInterface is the interface Name that uses an iSCSI transport. Defaults to 'default' (tcp).
  name: iscsiInterface
  type: string
- description: lun represents iSCSI Target Lun number.
  name: lun
  type: integer
- description: portals is the iSCSI Target Portal List. The portal is either an IP or ip_addr:port if the port is other than default (typically TCP ports 860 and 3260).
  name: portals
  type: array
- description: readOnly here will force the ReadOnly setting in VolumeMounts. Defaults to false.
  name: readOnly
  type: boolean
- description: secretRef is the CHAP Secret for iSCSI target and initiator authentication
  name: secretRef
  type: object
- description: targetPortal is iSCSI Target Portal. The Portal is either an IP or ip_addr:port if the port is other than default (typically TCP ports 860 and 3260).
  name: targetPortal
  type: string
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-iscsi-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-iscsi-volume-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-iscsi-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.ISCSIVolumeSource\",\n  \"description\": \"Represents an ISCSI disk. ISCSI volumes can only be mounted as read/write once. ISCSI volumes support ownership management and SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"chapAuthDiscovery\": {\n      \"description\": \"chapAuthDiscovery defines whether support iSCSI Discovery CHAP authentication\",\n      \"type\": \"boolean\"\n    },\n    \"chapAuthSession\": {\n      \"description\": \"chapAuthSession defines whether support iSCSI Session CHAP authentication\",\n      \"type\": \"boolean\"\n    },\n    \"fsType\": {\n      \"description\": \"fsType is the filesystem type of the volume that you want to mount. Tip: Ensure that\
  \ the filesystem type is supported by the host operating system. Examples: \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". Implicitly inferred to be \\\"ext4\\\" if unspecified. More info: https://kubernetes.io/docs/concepts/storage/volumes#iscsi\",\n      \"type\": \"string\"\n    },\n    \"initiatorName\": {\n      \"description\": \"initiatorName is the custom iSCSI Initiator Name. If initiatorName is specified with iscsiInterface simultaneously, new iSCSI interface <target portal>:<volume name> will be created for the connection.\",\n      \"type\": \"string\"\n    },\n    \"iqn\": {\n      \"description\": \"iqn is the target iSCSI Qualified Name.\",\n      \"type\": \"string\"\n    },\n    \"iscsiInterface\": {\n      \"description\": \"iscsiInterface is the interface Name that uses an iSCSI transport. Defaults to 'default' (tcp).\",\n      \"type\": \"string\"\n    },\n    \"lun\": {\n      \"description\": \"lun represents iSCSI Target Lun number.\",\n      \"type\": \"integer\"\n   \
  \ },\n    \"portals\": {\n      \"description\": \"portals is the iSCSI Target Portal List. The portal is either an IP or ip_addr:port if the port is other than default (typically TCP ports 860 and 3260).\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"x-kubernetes-list-type\": \"atomic\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly here will force the ReadOnly setting in VolumeMounts. Defaults to false.\",\n      \"type\": \"boolean\"\n    },\n    \"secretRef\": {\n      \"description\": \"secretRef is the CHAP Secret for iSCSI target and initiator authentication\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.LocalObjectReference\"\n    },\n    \"targetPortal\": {\n      \"description\": \"targetPortal is iSCSI Target Portal. The Portal is either an IP or ip_addr:port if the port is other than default (typically TCP ports 860 and 3260).\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"\
  targetPortal\",\n    \"iqn\",\n    \"lun\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-iscsi-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.ISCSIVolumeSource
---
