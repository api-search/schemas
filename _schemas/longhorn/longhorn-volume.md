---
description: Schema for Longhorn distributed block storage volumes. Longhorn volumes provide persistent block storage for Kubernetes workloads with automatic replication, snapshots, and backup to external storage targets.
layout: schema
name: Longhorn Volume
properties_list:
- description: Unique name for the volume within the Longhorn namespace.
  name: name
  type: string
- description: Size of the volume in bytes as a string, e.g. '10737418240' for 10 GiB.
  name: size
  type: string
- description: Number of data replicas maintained across Longhorn nodes. Higher values increase durability but consume more storage.
  name: numberOfReplicas
  type: integer
- description: Current lifecycle state of the volume.
  name: state
  type: string
- description: Health status of the volume based on replica availability and data integrity.
  name: robustness
  type: string
- description: Frontend protocol used to expose the volume to workloads. blockdev is the most common.
  name: frontend
  type: string
- description: Volume access mode. rwo is ReadWriteOnce for a single pod; rwx is ReadWriteMany for multiple pods.
  name: accessMode
  type: string
- description: Data locality policy. disabled places replicas freely; best-effort prefers the attached node; strict-local forces one replica on the attached node.
  name: dataLocality
  type: string
- description: Automatic rebalancing policy for distributing replicas evenly across nodes.
  name: replicaAutoBalance
  type: string
- description: Whether the volume data is encrypted at rest using the configured encryption secret.
  name: encrypted
  type: boolean
- description: Whether the volume supports live migration between nodes.
  name: migratable
  type: boolean
- description: Name of a backing image to use as pre-populated base data for this volume.
  name: backingImage
  type: string
- description: Longhorn engine image currently in use by this volume.
  name: currentImage
  type: string
- description: Node tags to restrict which nodes can host replicas of this volume.
  name: nodeSelector
  type: array
- description: Disk tags to restrict which disks can host replicas of this volume.
  name: diskSelector
  type: array
- description: Recurring jobs and groups assigned to this volume for automated operations.
  name: recurringJobSelector
  type: array
- description: List of replica instances maintaining copies of this volume's data.
  name: replicas
  type: array
- description: Map of named health conditions for the volume.
  name: conditions
  type: object
- description: Kubernetes PVC and PV binding status for this volume.
  name: kubernetesStatus
  type: object
provider_name: Longhorn
provider_slug: longhorn
schema_file: json-schema/longhorn-volume-schema.json
slug: longhorn-volume
source_filename: longhorn-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://longhorn.io/schemas/volume.json\",\n  \"title\": \"Longhorn Volume\",\n  \"description\": \"Schema for Longhorn distributed block storage volumes. Longhorn volumes provide persistent block storage for Kubernetes workloads with automatic replication, snapshots, and backup to external storage targets.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"size\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name for the volume within the Longhorn namespace.\",\n      \"minLength\": 1,\n      \"maxLength\": 63,\n      \"pattern\": \"^[a-z0-9][a-z0-9\\\\-\\\\.]*[a-z0-9]$\"\n    },\n    \"size\": {\n      \"type\": \"string\",\n      \"description\": \"Size of the volume in bytes as a string, e.g. '10737418240' for 10 GiB.\",\n      \"pattern\": \"^[0-9]+$\"\n    },\n    \"numberOfReplicas\": {\n      \"type\": \"integer\",\n      \"\
  minimum\": 1,\n      \"maximum\": 20,\n      \"default\": 3,\n      \"description\": \"Number of data replicas maintained across Longhorn nodes. Higher values increase durability but consume more storage.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\"creating\", \"attached\", \"detached\", \"attaching\", \"detaching\", \"deleting\"],\n      \"description\": \"Current lifecycle state of the volume.\"\n    },\n    \"robustness\": {\n      \"type\": \"string\",\n      \"enum\": [\"healthy\", \"degraded\", \"faulted\", \"unknown\"],\n      \"description\": \"Health status of the volume based on replica availability and data integrity.\"\n    },\n    \"frontend\": {\n      \"type\": \"string\",\n      \"enum\": [\"blockdev\", \"iscsi\", \"nvmf\"],\n      \"default\": \"blockdev\",\n      \"description\": \"Frontend protocol used to expose the volume to workloads. blockdev is the most common.\"\n    },\n    \"accessMode\": {\n      \"type\": \"string\",\n     \
  \ \"enum\": [\"rwo\", \"rwx\"],\n      \"default\": \"rwo\",\n      \"description\": \"Volume access mode. rwo is ReadWriteOnce for a single pod; rwx is ReadWriteMany for multiple pods.\"\n    },\n    \"dataLocality\": {\n      \"type\": \"string\",\n      \"enum\": [\"disabled\", \"best-effort\", \"strict-local\"],\n      \"default\": \"disabled\",\n      \"description\": \"Data locality policy. disabled places replicas freely; best-effort prefers the attached node; strict-local forces one replica on the attached node.\"\n    },\n    \"replicaAutoBalance\": {\n      \"type\": \"string\",\n      \"enum\": [\"ignored\", \"disabled\", \"least-effort\", \"best-effort\"],\n      \"description\": \"Automatic rebalancing policy for distributing replicas evenly across nodes.\"\n    },\n    \"encrypted\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether the volume data is encrypted at rest using the configured encryption secret.\"\n    },\n    \"migratable\"\
  : {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether the volume supports live migration between nodes.\"\n    },\n    \"backingImage\": {\n      \"type\": \"string\",\n      \"description\": \"Name of a backing image to use as pre-populated base data for this volume.\"\n    },\n    \"currentImage\": {\n      \"type\": \"string\",\n      \"description\": \"Longhorn engine image currently in use by this volume.\"\n    },\n    \"nodeSelector\": {\n      \"type\": \"array\",\n      \"description\": \"Node tags to restrict which nodes can host replicas of this volume.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Node tag name.\"\n      }\n    },\n    \"diskSelector\": {\n      \"type\": \"array\",\n      \"description\": \"Disk tags to restrict which disks can host replicas of this volume.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Disk tag name.\"\n      }\n    },\n    \"recurringJobSelector\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"Recurring jobs and groups assigned to this volume for automated operations.\",\n      \"items\": { \"$ref\": \"#/$defs/RecurringJobRef\" }\n    },\n    \"replicas\": {\n      \"type\": \"array\",\n      \"description\": \"List of replica instances maintaining copies of this volume's data.\",\n      \"items\": { \"$ref\": \"#/$defs/Replica\" }\n    },\n    \"conditions\": {\n      \"type\": \"object\",\n      \"description\": \"Map of named health conditions for the volume.\",\n      \"additionalProperties\": { \"$ref\": \"#/$defs/Condition\" }\n    },\n    \"kubernetesStatus\": {\n      \"$ref\": \"#/$defs/KubernetesStatus\",\n      \"description\": \"Kubernetes PVC and PV binding status for this volume.\"\n    }\n  },\n  \"$defs\": {\n    \"Replica\": {\n      \"type\": \"object\",\n      \"description\": \"A Longhorn replica storing a copy of volume data on a specific node and disk.\",\n      \"properties\": {\n        \"name\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Unique name of the replica instance.\"\n        },\n        \"hostId\": {\n          \"type\": \"string\",\n          \"description\": \"Kubernetes node name where this replica is located.\"\n        },\n        \"diskID\": {\n          \"type\": \"string\",\n          \"description\": \"Disk identifier on the node where this replica's data is stored.\"\n        },\n        \"dataPath\": {\n          \"type\": \"string\",\n          \"description\": \"Full file system path to the replica data directory on the node.\"\n        },\n        \"mode\": {\n          \"type\": \"string\",\n          \"enum\": [\"RW\", \"WO\", \"ERR\"],\n          \"description\": \"Replica mode. RW means fully operational; WO means write-only during rebuilding; ERR means the replica has failed.\"\n        },\n        \"running\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the replica process is currently running.\"\
  \n        },\n        \"failedAt\": {\n          \"type\": \"string\",\n          \"description\": \"Timestamp when the replica last failed, if applicable.\"\n        }\n      }\n    },\n    \"Snapshot\": {\n      \"type\": \"object\",\n      \"description\": \"A point-in-time snapshot of a Longhorn volume.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Unique name of the snapshot within the volume.\"\n        },\n        \"created\": {\n          \"type\": \"string\",\n          \"description\": \"Timestamp when the snapshot was created.\"\n        },\n        \"size\": {\n          \"type\": \"string\",\n          \"description\": \"Storage consumed by this snapshot in bytes as a string.\"\n        },\n        \"parent\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the parent snapshot in the chain.\"\n        },\n        \"removed\": {\n          \"type\": \"\
  boolean\",\n          \"description\": \"Whether this snapshot has been marked for removal.\"\n        },\n        \"usercreated\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this snapshot was created manually. False indicates a system-created snapshot.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Labels applied to this snapshot.\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"description\": \"Label value.\"\n          }\n        }\n      }\n    },\n    \"RecurringJobRef\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a recurring job or group assigned to a volume.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the recurring job or group.\"\n        },\n        \"isGroup\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether this reference is to a group rather than an individual job.\"\n        }\n      }\n    },\n    \"RecurringJob\": {\n      \"type\": \"object\",\n      \"description\": \"A Longhorn recurring job for scheduling automated snapshot or backup operations.\",\n      \"required\": [\"name\", \"task\", \"cron\", \"retain\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Unique name of the recurring job.\",\n          \"maxLength\": 63\n        },\n        \"task\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"snapshot\",\n            \"snapshot-force-create\",\n            \"snapshot-cleanup\",\n            \"snapshot-delete\",\n            \"backup\",\n            \"backup-force-create\",\n            \"filesystem-trim\"\n          ],\n          \"description\": \"Type of operation this recurring job performs.\"\n        },\n        \"cron\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Cron expression defining the schedule, e.g. '0 2 * * *' for 2:00 AM daily.\"\n        },\n        \"retain\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of snapshots or backups to retain. Older items are automatically deleted.\"\n        },\n        \"concurrency\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"default\": 1,\n          \"description\": \"Maximum number of volumes to process simultaneously when this job fires.\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Labels to apply to snapshots or backups created by this job.\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"description\": \"Label value.\"\n          }\n        },\n        \"groups\": {\n          \"type\": \"array\",\n          \"description\": \"Group names this job belongs to. Volumes assigned to the group will be\
  \ processed.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"Group name.\"\n          }\n        }\n      }\n    },\n    \"Node\": {\n      \"type\": \"object\",\n      \"description\": \"A Longhorn storage node participating in the cluster.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Node identifier, matching the Kubernetes node name.\"\n        },\n        \"allowScheduling\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether new replicas can be scheduled on this node.\"\n        },\n        \"evictionRequested\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether replica eviction has been requested for this node.\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"Tags applied to this node for workload placement affinity.\",\n          \"items\": {\n\
  \            \"type\": \"string\",\n            \"description\": \"Tag value.\"\n          }\n        },\n        \"disks\": {\n          \"type\": \"object\",\n          \"description\": \"Map of disk configurations on this node keyed by disk name.\",\n          \"additionalProperties\": { \"$ref\": \"#/$defs/DiskSpec\" }\n        },\n        \"conditions\": {\n          \"type\": \"object\",\n          \"description\": \"Health conditions for the node.\",\n          \"additionalProperties\": { \"$ref\": \"#/$defs/Condition\" }\n        }\n      }\n    },\n    \"DiskSpec\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for a disk available for Longhorn replica storage.\",\n      \"required\": [\"path\"],\n      \"properties\": {\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"File system path to the disk or directory used for Longhorn storage.\"\n        },\n        \"allowScheduling\": {\n          \"type\": \"boolean\",\n\
  \          \"description\": \"Whether new replicas can be scheduled on this disk.\"\n        },\n        \"evictionRequested\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether eviction of replicas from this disk has been requested.\"\n        },\n        \"storageReserved\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Storage in bytes reserved for non-Longhorn use on this disk.\"\n        },\n        \"tags\": {\n          \"type\": \"array\",\n          \"description\": \"Tags for disk affinity in volume and replica placement.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"Tag value.\"\n          }\n        }\n      }\n    },\n    \"Condition\": {\n      \"type\": \"object\",\n      \"description\": \"A health condition for a Longhorn resource.\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"True\", \"False\"\
  , \"Unknown\"],\n          \"description\": \"Status of the condition.\"\n        },\n        \"reason\": {\n          \"type\": \"string\",\n          \"description\": \"Machine-readable reason for the condition.\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable message for the condition.\"\n        },\n        \"lastProbeTime\": {\n          \"type\": \"string\",\n          \"description\": \"Timestamp of the last condition probe.\"\n        },\n        \"lastTransitionTime\": {\n          \"type\": \"string\",\n          \"description\": \"Timestamp of the last condition transition.\"\n        }\n      }\n    },\n    \"KubernetesStatus\": {\n      \"type\": \"object\",\n      \"description\": \"Kubernetes PVC and PV binding status for a Longhorn volume.\",\n      \"properties\": {\n        \"pvName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the Kubernetes PersistentVolume bound to this\
  \ Longhorn volume.\"\n        },\n        \"pvStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the PersistentVolume.\"\n        },\n        \"pvcName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the Kubernetes PersistentVolumeClaim using this volume.\"\n        },\n        \"namespace\": {\n          \"type\": \"string\",\n          \"description\": \"Namespace of the PVC.\"\n        },\n        \"lastPVCRefAt\": {\n          \"type\": \"string\",\n          \"description\": \"Timestamp when the PVC was last bound.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/json-schema/longhorn-volume-schema.json
tags:
- Backup
- Block Storage
- Cloud Native
- Incubating
- Kubernetes
- Persistent Volumes
title: Longhorn Volume
---
