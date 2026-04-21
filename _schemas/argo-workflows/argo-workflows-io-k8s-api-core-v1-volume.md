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
