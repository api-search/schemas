---
description: Volume represents a named volume in a pod that may be accessed by any container in the pod.
layout: schema
name: io.k8s.api.core.v1.Volume
properties_list:
- description: 'awsElasticBlockStore represents an AWS Disk resource that is attached to a kubelet''s host machine and then exposed to the pod. Deprecated: AWSElasticBlockStore is deprecated. All operations for the in'
  name: awsElasticBlockStore
  type: object
- description: 'azureDisk represents an Azure Data Disk mount on the host and bind mount to the pod. Deprecated: AzureDisk is deprecated. All operations for the in-tree azureDisk type are redirected to the disk.csi.a'
  name: azureDisk
  type: object
- description: 'azureFile represents an Azure File Service mount on the host and bind mount to the pod. Deprecated: AzureFile is deprecated. All operations for the in-tree azureFile type are redirected to the file.cs'
  name: azureFile
  type: object
- description: 'cephFS represents a Ceph FS mount on the host that shares a pod''s lifetime. Deprecated: CephFS is deprecated and the in-tree cephfs type is no longer supported.'
  name: cephfs
  type: object
- description: 'cinder represents a cinder volume attached and mounted on kubelets host machine. Deprecated: Cinder is deprecated. All operations for the in-tree cinder type are redirected to the cinder.csi.openstack'
  name: cinder
  type: object
- description: configMap represents a configMap that should populate this volume
  name: configMap
  type: object
- description: csi (Container Storage Interface) represents ephemeral storage that is handled by certain external CSI drivers.
  name: csi
  type: object
- description: downwardAPI represents downward API about the pod that should populate this volume
  name: downwardAPI
  type: object
- description: 'emptyDir represents a temporary directory that shares a pod''s lifetime. More info: https://kubernetes.io/docs/concepts/storage/volumes#emptydir'
  name: emptyDir
  type: object
- description: ephemeral represents a volume that is handled by a cluster storage driver. The volume's lifecycle is tied to the pod that defines it - it will be created before the pod starts, and deleted when the po
  name: ephemeral
  type: object
- description: fc represents a Fibre Channel resource that is attached to a kubelet's host machine and then exposed to the pod.
  name: fc
  type: object
- description: 'flexVolume represents a generic volume resource that is provisioned/attached using an exec based plugin. Deprecated: FlexVolume is deprecated. Consider using a CSIDriver instead.'
  name: flexVolume
  type: object
- description: 'flocker represents a Flocker volume attached to a kubelet''s host machine. This depends on the Flocker control service being running. Deprecated: Flocker is deprecated and the in-tree flocker type is n'
  name: flocker
  type: object
- description: 'gcePersistentDisk represents a GCE Disk resource that is attached to a kubelet''s host machine and then exposed to the pod. Deprecated: GCEPersistentDisk is deprecated. All operations for the in-tree g'
  name: gcePersistentDisk
  type: object
- description: 'gitRepo represents a git repository at a particular revision. Deprecated: GitRepo is deprecated. To provision a container with a git repo, mount an EmptyDir into an InitContainer that clones the repo '
  name: gitRepo
  type: object
- description: 'glusterfs represents a Glusterfs mount on the host that shares a pod''s lifetime. Deprecated: Glusterfs is deprecated and the in-tree glusterfs type is no longer supported.'
  name: glusterfs
  type: object
- description: hostPath represents a pre-existing file or directory on the host machine that is directly exposed to the container. This is generally used for system agents or other privileged things that are allowed
  name: hostPath
  type: object
- description: 'image represents an OCI object (a container image or artifact) pulled and mounted on the kubelet''s host machine. The volume is resolved at pod startup depending on which PullPolicy value is provided: '
  name: image
  type: object
- description: 'iscsi represents an ISCSI Disk resource that is attached to a kubelet''s host machine and then exposed to the pod. More info: https://kubernetes.io/docs/concepts/storage/volumes/#iscsi'
  name: iscsi
  type: object
- description: 'name of the volume. Must be a DNS_LABEL and unique within the pod. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names'
  name: name
  type: string
- description: 'nfs represents an NFS mount on the host that shares a pod''s lifetime More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs'
  name: nfs
  type: object
- description: 'persistentVolumeClaimVolumeSource represents a reference to a PersistentVolumeClaim in the same namespace. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumecla'
  name: persistentVolumeClaim
  type: object
- description: 'photonPersistentDisk represents a PhotonController persistent disk attached and mounted on kubelets host machine. Deprecated: PhotonPersistentDisk is deprecated and the in-tree photonPersistentDisk ty'
  name: photonPersistentDisk
  type: object
- description: 'portworxVolume represents a portworx volume attached and mounted on kubelets host machine. Deprecated: PortworxVolume is deprecated. All operations for the in-tree portworxVolume type are redirected t'
  name: portworxVolume
  type: object
- description: projected items for all in one resources secrets, configmaps, and downward API
  name: projected
  type: object
- description: 'quobyte represents a Quobyte mount on the host that shares a pod''s lifetime. Deprecated: Quobyte is deprecated and the in-tree quobyte type is no longer supported.'
  name: quobyte
  type: object
- description: 'rbd represents a Rados Block Device mount on the host that shares a pod''s lifetime. Deprecated: RBD is deprecated and the in-tree rbd type is no longer supported.'
  name: rbd
  type: object
- description: 'scaleIO represents a ScaleIO persistent volume attached and mounted on Kubernetes nodes. Deprecated: ScaleIO is deprecated and the in-tree scaleIO type is no longer supported.'
  name: scaleIO
  type: object
- description: 'secret represents a secret that should populate this volume. More info: https://kubernetes.io/docs/concepts/storage/volumes#secret'
  name: secret
  type: object
- description: 'storageOS represents a StorageOS volume attached and mounted on Kubernetes nodes. Deprecated: StorageOS is deprecated and the in-tree storageos type is no longer supported.'
  name: storageos
  type: object
- description: 'vsphereVolume represents a vSphere volume attached and mounted on kubelets host machine. Deprecated: VsphereVolume is deprecated. All operations for the in-tree vsphereVolume type are redirected to th'
  name: vsphereVolume
  type: object
provider_name: Argo Workflows
provider_slug: argo-workflows
schema_file: json-schema/argo-workflows-io-k8s-api-core-v1-volume-schema.json
slug: argo-workflows-io-k8s-api-core-v1-volume
source_filename: argo-workflows-io-k8s-api-core-v1-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-volume-schema.json\",\n  \"title\": \"io.k8s.api.core.v1.Volume\",\n  \"description\": \"Volume represents a named volume in a pod that may be accessed by any container in the pod.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsElasticBlockStore\": {\n      \"description\": \"awsElasticBlockStore represents an AWS Disk resource that is attached to a kubelet's host machine and then exposed to the pod. Deprecated: AWSElasticBlockStore is deprecated. All operations for the in-tree awsElasticBlockStore type are redirected to the ebs.csi.aws.com CSI driver. More info: https://kubernetes.io/docs/concepts/storage/volumes#awselasticblockstore\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.AWSElasticBlockStoreVolumeSource\"\n    },\n    \"azureDisk\": {\n   \
  \   \"description\": \"azureDisk represents an Azure Data Disk mount on the host and bind mount to the pod. Deprecated: AzureDisk is deprecated. All operations for the in-tree azureDisk type are redirected to the disk.csi.azure.com CSI driver.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.AzureDiskVolumeSource\"\n    },\n    \"azureFile\": {\n      \"description\": \"azureFile represents an Azure File Service mount on the host and bind mount to the pod. Deprecated: AzureFile is deprecated. All operations for the in-tree azureFile type are redirected to the file.csi.azure.com CSI driver.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.AzureFileVolumeSource\"\n    },\n    \"cephfs\": {\n      \"description\": \"cephFS represents a Ceph FS mount on the host that shares a pod's lifetime. Deprecated: CephFS is deprecated and the in-tree cephfs type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.CephFSVolumeSource\"\n    },\n    \"cinder\": {\n\
  \      \"description\": \"cinder represents a cinder volume attached and mounted on kubelets host machine. Deprecated: Cinder is deprecated. All operations for the in-tree cinder type are redirected to the cinder.csi.openstack.org CSI driver. More info: https://examples.k8s.io/mysql-cinder-pd/README.md\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.CinderVolumeSource\"\n    },\n    \"configMap\": {\n      \"description\": \"configMap represents a configMap that should populate this volume\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ConfigMapVolumeSource\"\n    },\n    \"csi\": {\n      \"description\": \"csi (Container Storage Interface) represents ephemeral storage that is handled by certain external CSI drivers.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.CSIVolumeSource\"\n    },\n    \"downwardAPI\": {\n      \"description\": \"downwardAPI represents downward API about the pod that should populate this volume\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.DownwardAPIVolumeSource\"\
  \n    },\n    \"emptyDir\": {\n      \"description\": \"emptyDir represents a temporary directory that shares a pod's lifetime. More info: https://kubernetes.io/docs/concepts/storage/volumes#emptydir\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.EmptyDirVolumeSource\"\n    },\n    \"ephemeral\": {\n      \"description\": \"ephemeral represents a volume that is handled by a cluster storage driver. The volume's lifecycle is tied to the pod that defines it - it will be created before the pod starts, and deleted when the pod is removed.\\n\\nUse this if: a) the volume is only needed while the pod runs, b) features of normal volumes like restoring from snapshot or capacity\\n   tracking are needed,\\nc) the storage driver is specified through a storage class, and d) the storage driver supports dynamic volume provisioning through\\n   a PersistentVolumeClaim (see EphemeralVolumeSource for more\\n   information on the connection between this volume type\\n   and PersistentVolumeClaim).\\\
  n\\nUse PersistentVolumeClaim or one of the vendor-specific APIs for volumes that persist for longer than the lifecycle of an individual pod.\\n\\nUse CSI for light-weight local ephemeral volumes if the CSI driver is meant to be used that way - see the documentation of the driver for more information.\\n\\nA pod can use both types of ephemeral volumes and persistent volumes at the same time.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.EphemeralVolumeSource\"\n    },\n    \"fc\": {\n      \"description\": \"fc represents a Fibre Channel resource that is attached to a kubelet's host machine and then exposed to the pod.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.FCVolumeSource\"\n    },\n    \"flexVolume\": {\n      \"description\": \"flexVolume represents a generic volume resource that is provisioned/attached using an exec based plugin. Deprecated: FlexVolume is deprecated. Consider using a CSIDriver instead.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.FlexVolumeSource\"\
  \n    },\n    \"flocker\": {\n      \"description\": \"flocker represents a Flocker volume attached to a kubelet's host machine. This depends on the Flocker control service being running. Deprecated: Flocker is deprecated and the in-tree flocker type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.FlockerVolumeSource\"\n    },\n    \"gcePersistentDisk\": {\n      \"description\": \"gcePersistentDisk represents a GCE Disk resource that is attached to a kubelet's host machine and then exposed to the pod. Deprecated: GCEPersistentDisk is deprecated. All operations for the in-tree gcePersistentDisk type are redirected to the pd.csi.storage.gke.io CSI driver. More info: https://kubernetes.io/docs/concepts/storage/volumes#gcepersistentdisk\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.GCEPersistentDiskVolumeSource\"\n    },\n    \"gitRepo\": {\n      \"description\": \"gitRepo represents a git repository at a particular revision. Deprecated: GitRepo is\
  \ deprecated. To provision a container with a git repo, mount an EmptyDir into an InitContainer that clones the repo using git, then mount the EmptyDir into the Pod's container.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.GitRepoVolumeSource\"\n    },\n    \"glusterfs\": {\n      \"description\": \"glusterfs represents a Glusterfs mount on the host that shares a pod's lifetime. Deprecated: Glusterfs is deprecated and the in-tree glusterfs type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.GlusterfsVolumeSource\"\n    },\n    \"hostPath\": {\n      \"description\": \"hostPath represents a pre-existing file or directory on the host machine that is directly exposed to the container. This is generally used for system agents or other privileged things that are allowed to see the host machine. Most containers will NOT need this. More info: https://kubernetes.io/docs/concepts/storage/volumes#hostpath\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.HostPathVolumeSource\"\
  \n    },\n    \"image\": {\n      \"description\": \"image represents an OCI object (a container image or artifact) pulled and mounted on the kubelet's host machine. The volume is resolved at pod startup depending on which PullPolicy value is provided:\\n\\n- Always: the kubelet always attempts to pull the reference. Container creation will fail If the pull fails. - Never: the kubelet never pulls the reference and only uses a local image or artifact. Container creation will fail if the reference isn't present. - IfNotPresent: the kubelet pulls if the reference isn't already present on disk. Container creation will fail if the reference isn't present and the pull fails.\\n\\nThe volume gets re-resolved if the pod gets deleted and recreated, which means that new remote content will become available on pod recreation. A failure to resolve or pull the image during pod startup will block containers from starting and may add significant latency. Failures will be retried using normal volume backoff\
  \ and will be reported on the pod reason and message. The types of objects that may be mounted by this volume are defined by the container runtime implementation on a host machine and at minimum must include all valid types supported by the container image field. The OCI object gets mounted in a single directory (spec.containers[*].volumeMounts.mountPath) by merging the manifest layers in the same way as for container images. The volume will be mounted read-only (ro) and non-executable files (noexec). Sub path mounts for containers are not supported (spec.containers[*].volumeMounts.subpath) before 1.33. The field spec.securityContext.fsGroupChangePolicy has no effect on this volume type.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ImageVolumeSource\"\n    },\n    \"iscsi\": {\n      \"description\": \"iscsi represents an ISCSI Disk resource that is attached to a kubelet's host machine and then exposed to the pod. More info: https://kubernetes.io/docs/concepts/storage/volumes/#iscsi\"\
  ,\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ISCSIVolumeSource\"\n    },\n    \"name\": {\n      \"description\": \"name of the volume. Must be a DNS_LABEL and unique within the pod. More info: https://kubernetes.io/docs/concepts/overview/working-with-objects/names/#names\",\n      \"type\": \"string\"\n    },\n    \"nfs\": {\n      \"description\": \"nfs represents an NFS mount on the host that shares a pod's lifetime More info: https://kubernetes.io/docs/concepts/storage/volumes#nfs\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.NFSVolumeSource\"\n    },\n    \"persistentVolumeClaim\": {\n      \"description\": \"persistentVolumeClaimVolumeSource represents a reference to a PersistentVolumeClaim in the same namespace. More info: https://kubernetes.io/docs/concepts/storage/persistent-volumes#persistentvolumeclaims\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PersistentVolumeClaimVolumeSource\"\n    },\n    \"photonPersistentDisk\": {\n      \"description\":\
  \ \"photonPersistentDisk represents a PhotonController persistent disk attached and mounted on kubelets host machine. Deprecated: PhotonPersistentDisk is deprecated and the in-tree photonPersistentDisk type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PhotonPersistentDiskVolumeSource\"\n    },\n    \"portworxVolume\": {\n      \"description\": \"portworxVolume represents a portworx volume attached and mounted on kubelets host machine. Deprecated: PortworxVolume is deprecated. All operations for the in-tree portworxVolume type are redirected to the pxd.portworx.com CSI driver when the CSIMigrationPortworx feature-gate is on.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.PortworxVolumeSource\"\n    },\n    \"projected\": {\n      \"description\": \"projected items for all in one resources secrets, configmaps, and downward API\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ProjectedVolumeSource\"\n    },\n    \"quobyte\": {\n      \"description\"\
  : \"quobyte represents a Quobyte mount on the host that shares a pod's lifetime. Deprecated: Quobyte is deprecated and the in-tree quobyte type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.QuobyteVolumeSource\"\n    },\n    \"rbd\": {\n      \"description\": \"rbd represents a Rados Block Device mount on the host that shares a pod's lifetime. Deprecated: RBD is deprecated and the in-tree rbd type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.RBDVolumeSource\"\n    },\n    \"scaleIO\": {\n      \"description\": \"scaleIO represents a ScaleIO persistent volume attached and mounted on Kubernetes nodes. Deprecated: ScaleIO is deprecated and the in-tree scaleIO type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.ScaleIOVolumeSource\"\n    },\n    \"secret\": {\n      \"description\": \"secret represents a secret that should populate this volume. More info: https://kubernetes.io/docs/concepts/storage/volumes#secret\"\
  ,\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.SecretVolumeSource\"\n    },\n    \"storageos\": {\n      \"description\": \"storageOS represents a StorageOS volume attached and mounted on Kubernetes nodes. Deprecated: StorageOS is deprecated and the in-tree storageos type is no longer supported.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.StorageOSVolumeSource\"\n    },\n    \"vsphereVolume\": {\n      \"description\": \"vsphereVolume represents a vSphere volume attached and mounted on kubelets host machine. Deprecated: VsphereVolume is deprecated. All operations for the in-tree vsphereVolume type are redirected to the csi.vsphere.vmware.com CSI driver.\",\n      \"$ref\": \"#/definitions/io.k8s.api.core.v1.VsphereVirtualDiskVolumeSource\"\n    }\n  },\n  \"required\": [\n    \"name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-workflows/refs/heads/main/json-schema/argo-workflows-io-k8s-api-core-v1-volume-schema.json
tags:
- CNCF
- Containers
- Data Processing
- Kubernetes
- Machine Learning
- Open Source
- Workflow Engine
title: io.k8s.api.core.v1.Volume
---
