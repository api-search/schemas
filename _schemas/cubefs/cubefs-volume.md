---
description: Schema for CubeFS volume configuration and status. Volumes are the top-level storage namespaces in CubeFS that can be accessed via POSIX, HDFS, or S3-compatible interfaces. Each volume owns a set of data partitions and metadata partitions distributed across the cluster.
layout: schema
name: CubeFS Volume
properties_list:
- description: Unique name identifying the volume within the CubeFS cluster. Also used as the S3 bucket name.
  name: name
  type: string
- description: User ID that owns this volume. The owner has full control permissions.
  name: owner
  type: string
- description: Total storage capacity allocated to this volume in gigabytes.
  name: capacity
  type: integer
- description: Replication factor for data partitions. Replicated volumes only. 3 is the standard for high availability.
  name: replicaNum
  type: integer
- description: Volume type. 0 for replicated volumes; 1 for erasure-coded (EC) volumes.
  name: volType
  type: integer
- description: Initial number of metadata partitions to create. Each metadata partition stores inode and directory entry data.
  name: mpCount
  type: integer
- description: Initial number of data partitions to create. Data partitions store the actual file data blocks.
  name: dpCount
  type: integer
- description: Whether follower replicas can serve read requests. Enabling this improves read throughput at the cost of potentially serving slightly stale data.
  name: followerRead
  type: boolean
- description: Whether POSIX access control lists are enabled on this volume. Required for multi-user POSIX permission support.
  name: enablePosixAcl
  type: boolean
- description: Whether quality of service throttling is enabled on this volume to limit bandwidth and IOPS.
  name: qosEnable
  type: boolean
- description: Current volume status. 0 means normal and active; 1 means marked for deletion.
  name: status
  type: integer
- description: Timestamp when the volume was created.
  name: createTime
  type: string
- description: Optional human-readable description of the volume's purpose.
  name: description
  type: string
- description: List of data partitions belonging to this volume.
  name: dataPartitions
  type: array
- description: List of metadata partitions belonging to this volume.
  name: metaPartitions
  type: array
- description: Currently used storage in bytes.
  name: usedSize
  type: integer
- description: Total allocated storage capacity in bytes.
  name: totalSize
  type: integer
provider_name: CubeFS
provider_slug: cubefs
schema_file: json-schema/cubefs-volume-schema.json
slug: cubefs-volume
source_filename: cubefs-volume-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cubefs.io/schemas/volume.json\",\n  \"title\": \"CubeFS Volume\",\n  \"description\": \"Schema for CubeFS volume configuration and status. Volumes are the top-level storage namespaces in CubeFS that can be accessed via POSIX, HDFS, or S3-compatible interfaces. Each volume owns a set of data partitions and metadata partitions distributed across the cluster.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"owner\", \"capacity\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name identifying the volume within the CubeFS cluster. Also used as the S3 bucket name.\",\n      \"minLength\": 1,\n      \"maxLength\": 256,\n      \"pattern\": \"^[a-zA-Z0-9][a-zA-Z0-9_\\\\-\\\\.]*$\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"User ID that owns this volume. The owner has full control permissions.\"\
  ,\n      \"minLength\": 1\n    },\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"description\": \"Total storage capacity allocated to this volume in gigabytes.\"\n    },\n    \"replicaNum\": {\n      \"type\": \"integer\",\n      \"enum\": [1, 2, 3],\n      \"default\": 3,\n      \"description\": \"Replication factor for data partitions. Replicated volumes only. 3 is the standard for high availability.\"\n    },\n    \"volType\": {\n      \"type\": \"integer\",\n      \"enum\": [0, 1],\n      \"default\": 0,\n      \"description\": \"Volume type. 0 for replicated volumes; 1 for erasure-coded (EC) volumes.\"\n    },\n    \"mpCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"default\": 3,\n      \"description\": \"Initial number of metadata partitions to create. Each metadata partition stores inode and directory entry data.\"\n    },\n    \"dpCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 1,\n      \"default\": 10,\n\
  \      \"description\": \"Initial number of data partitions to create. Data partitions store the actual file data blocks.\"\n    },\n    \"followerRead\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether follower replicas can serve read requests. Enabling this improves read throughput at the cost of potentially serving slightly stale data.\"\n    },\n    \"enablePosixAcl\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether POSIX access control lists are enabled on this volume. Required for multi-user POSIX permission support.\"\n    },\n    \"qosEnable\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether quality of service throttling is enabled on this volume to limit bandwidth and IOPS.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"enum\": [0, 1],\n      \"description\": \"Current volume status. 0 means normal and active; 1 means marked\
  \ for deletion.\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the volume was created.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Optional human-readable description of the volume's purpose.\"\n    },\n    \"dataPartitions\": {\n      \"type\": \"array\",\n      \"description\": \"List of data partitions belonging to this volume.\",\n      \"items\": { \"$ref\": \"#/$defs/DataPartition\" }\n    },\n    \"metaPartitions\": {\n      \"type\": \"array\",\n      \"description\": \"List of metadata partitions belonging to this volume.\",\n      \"items\": { \"$ref\": \"#/$defs/MetaPartition\" }\n    },\n    \"usedSize\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Currently used storage in bytes.\"\n    },\n    \"totalSize\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Total allocated storage capacity in bytes.\"\n  \
  \  }\n  },\n  \"$defs\": {\n    \"DataPartition\": {\n      \"type\": \"object\",\n      \"description\": \"A data partition within a CubeFS volume that stores actual file data blocks.\",\n      \"required\": [\"partitionID\"],\n      \"properties\": {\n        \"partitionID\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique identifier for this data partition.\"\n        },\n        \"status\": {\n          \"type\": \"integer\",\n          \"description\": \"Partition status. 1 is read-write; 2 is read-only; 3 is unavailable.\"\n        },\n        \"replicaNum\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of replicas for this partition.\"\n        },\n        \"hosts\": {\n          \"type\": \"array\",\n          \"description\": \"List of data node addresses hosting replicas of this partition.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"Data node address in host:port format.\"\n\
  \          }\n        },\n        \"isRecover\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this partition is currently in a recovery state.\"\n        },\n        \"total\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total capacity of this partition in bytes.\"\n        },\n        \"used\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Used capacity of this partition in bytes.\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Disk path on the data node where this partition's data is stored.\"\n        }\n      }\n    },\n    \"MetaPartition\": {\n      \"type\": \"object\",\n      \"description\": \"A metadata partition within a CubeFS volume that stores inode and directory entry data.\",\n      \"required\": [\"partitionID\"],\n      \"properties\": {\n        \"partitionID\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Unique identifier for this metadata partition.\"\n        },\n        \"start\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Start of the inode number range managed by this partition.\"\n        },\n        \"end\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"End of the inode number range managed by this partition.\"\n        },\n        \"inodeCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Current number of inodes stored in this partition.\"\n        },\n        \"maxInodeID\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The highest inode ID currently allocated in this partition.\"\n        },\n        \"isRecover\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this metadata partition is currently recovering.\"\n        },\n \
  \       \"hosts\": {\n          \"type\": \"array\",\n          \"description\": \"List of metadata node addresses hosting this partition.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"Metadata node address in host:port format.\"\n          }\n        },\n        \"leader\": {\n          \"type\": \"string\",\n          \"description\": \"Address of the current raft leader for this partition.\"\n        }\n      }\n    },\n    \"User\": {\n      \"type\": \"object\",\n      \"description\": \"A CubeFS user account with S3 credentials and volume ownership.\",\n      \"required\": [\"user_id\"],\n      \"properties\": {\n        \"user_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique user identifier within the CubeFS cluster.\",\n          \"minLength\": 1\n        },\n        \"access_key\": {\n          \"type\": \"string\",\n          \"description\": \"S3-compatible access key for authenticating object storage\
  \ requests.\",\n          \"minLength\": 16\n        },\n        \"secret_key\": {\n          \"type\": \"string\",\n          \"description\": \"S3-compatible secret key for signing object storage requests.\",\n          \"minLength\": 32\n        },\n        \"own_vols\": {\n          \"type\": \"array\",\n          \"description\": \"List of volume names that this user owns.\",\n          \"items\": {\n            \"type\": \"string\",\n            \"description\": \"Volume name.\"\n          }\n        },\n        \"authorized_vols\": {\n          \"type\": \"object\",\n          \"description\": \"Map of volume names to access permission levels granted to this user.\",\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"enum\": [\"READONLY\", \"RO\", \"READWRITE\", \"RW\", \"NONE\"],\n            \"description\": \"Permission level on the volume.\"\n          }\n        },\n        \"user_type\": {\n          \"type\": \"integer\",\n          \"\
  enum\": [0, 1],\n          \"description\": \"User type. 0 for normal user; 1 for admin user with cluster-wide privileges.\"\n        },\n        \"create_time\": {\n          \"type\": \"string\",\n          \"description\": \"Timestamp when the user account was created.\"\n        }\n      }\n    },\n    \"DataNode\": {\n      \"type\": \"object\",\n      \"description\": \"A CubeFS data node that stores data partition replicas.\",\n      \"required\": [\"addr\"],\n      \"properties\": {\n        \"addr\": {\n          \"type\": \"string\",\n          \"description\": \"Network address of the data node in host:port format.\",\n          \"pattern\": \"^[^:]+:[0-9]+$\"\n        },\n        \"status\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this node is currently active and healthy.\"\n        },\n        \"isWritable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this node can accept new data partition allocations.\"\n\
  \        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique numeric identifier assigned to this node by the Master.\"\n        },\n        \"totalWeight\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total storage capacity of this node in bytes.\"\n        },\n        \"usedWeight\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Used storage on this node in bytes.\"\n        },\n        \"availableSpace\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Available storage remaining on this node in bytes.\"\n        },\n        \"dataPartitionCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of data partitions currently hosted on this node.\"\n        }\n      }\n    },\n    \"MetaNode\": {\n      \"type\": \"object\",\n      \"description\": \"A CubeFS\
  \ metadata node that stores metadata partition data.\",\n      \"required\": [\"addr\"],\n      \"properties\": {\n        \"addr\": {\n          \"type\": \"string\",\n          \"description\": \"Network address of the metadata node in host:port format.\",\n          \"pattern\": \"^[^:]+:[0-9]+$\"\n        },\n        \"status\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this node is currently active and healthy.\"\n        },\n        \"isWritable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this node can accept new metadata partition allocations.\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Unique numeric identifier assigned to this node by the Master.\"\n        },\n        \"totalWeight\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total memory or storage capacity of this node in bytes.\"\n        },\n        \"usedWeight\"\
  : {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Used memory or storage on this node in bytes.\"\n        },\n        \"metaPartitionCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of metadata partitions currently hosted on this node.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/json-schema/cubefs-volume-schema.json
tags:
- Cloud Native
- CNCF Graduated
- Distributed File System
- Kubernetes
- Object Storage
- POSIX
- S3 Compatible
- Storage
title: CubeFS Volume
---
