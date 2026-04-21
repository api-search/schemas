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
