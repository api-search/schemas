---
description: Represents a Persistent Disk resource in Google Compute Engine. A GCE PD must exist before mounting to a container. The disk must also be in the same GCE project and zone as the kubelet. A GCE PD can only be mounted as read/write once or read-only many times. GCE PDs support ownership management and SELinux relabeling.
layout: schema
name: io.k8s.api.core.v1.GCEPersistentDiskVolumeSource
properties_list:
- description: 'fsType is filesystem type of the volume that you want to mount. Tip: Ensure that the filesystem type is supported by the host operating system. Examples: "ext4", "xfs", "ntfs". Implicitly inferred to '
  name: fsType
  type: string
- description: 'partition is the partition in the volume that you want to mount. If omitted, the default is to mount by volume name. Examples: For volume /dev/sda1, you specify the partition as "1". Similarly, the vo'
  name: partition
  type: integer
- description: 'pdName is unique name of the PD resource in GCE. Used to identify the disk in GCE. More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk'
  name: pdName
  type: string
- description: 'readOnly here will force the ReadOnly setting in VolumeMounts. Defaults to false. More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk'
  name: readOnly
  type: boolean
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-gce-persistent-disk-volume-source-schema.json
slug: argo-workflows-io-k8s-api-core-v1-gce-persistent-disk-volume-source
source_filename: argo-workflows-io-k8s-api-core-v1-gce-persistent-disk-volume-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-gce-persistent-disk-volume-source-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.GCEPersistentDiskVolumeSource\",\n  \"description\": \"Represents a Persistent Disk resource in Google Compute Engine.\\n\\nA GCE PD must exist before mounting to a container. The disk must also be in the same GCE project and zone as the kubelet. A GCE PD can only be mounted as read/write once or read-only many times. GCE PDs support ownership management and SELinux relabeling.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fsType\": {\n      \"description\": \"fsType is filesystem type of the volume that you want to mount. Tip: Ensure that the filesystem type is supported by the host operating system. Examples: \\\"ext4\\\", \\\"xfs\\\", \\\"ntfs\\\". Implicitly inferred to be\
  \ \\\"ext4\\\" if unspecified. More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk\",\n      \"type\": \"string\"\n    },\n    \"partition\": {\n      \"description\": \"partition is the partition in the volume that you want to mount. If omitted, the default is to mount by volume name. Examples: For volume /dev/sda1, you specify the partition as \\\"1\\\". Similarly, the volume partition for /dev/sda is \\\"0\\\" (or you can leave the property empty). More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk\",\n      \"type\": \"integer\"\n    },\n    \"pdName\": {\n      \"description\": \"pdName is unique name of the PD resource in GCE. Used to identify the disk in GCE. More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk\",\n      \"type\": \"string\"\n    },\n    \"readOnly\": {\n      \"description\": \"readOnly here will force the ReadOnly setting in VolumeMounts. Defaults to false. More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk\"\
  ,\n      \"type\": \"boolean\"\n    }\n  },\n  \"required\": [\n    \"pdName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-gce-persistent-disk-volume-source-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.GCEPersistentDiskVolumeSource
---
