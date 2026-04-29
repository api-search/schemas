---
description: Represents a complete Solaris zone configuration including global properties, resource assignments, and networking for non-global zones managed through zonecfg(8) and the RAD zonemgr module.
layout: schema
name: Oracle Solaris Zone Configuration
properties_list:
- description: Unique name identifying the zone on the system
  name: name
  type: string
- description: Universally unique identifier assigned to the zone
  name: uuid
  type: string
- description: Zone brand determining the runtime environment and kernel behavior
  name: brand
  type: string
- description: File system path for the zone root directory
  name: zonepath
  type: string
- description: Whether the zone should automatically boot when the global zone boots
  name: autoboot
  type: boolean
- description: Action to take when the global zone is shut down
  name: autoshutdown
  type: string
- description: Boot arguments passed to the zone at boot time
  name: bootargs
  type: string
- description: File MAC policy profile for mandatory access control
  name: file-mac-profile
  type: string
- description: Emulated host identifier for the zone
  name: hostid
  type: string
- description: IP stack type for the zone
  name: ip-type
  type: string
- description: Comma-separated list of privileges for the zone
  name: limitpriv
  type: string
- description: Default scheduling class for processes in the zone
  name: scheduling-class
  type: string
- description: Maximum number of lightweight processes allowed in the zone
  name: max-lwps
  type: integer
- description: Maximum number of processes allowed in the zone
  name: max-processes
  type: integer
- description: Maximum shared memory allowed for the zone
  name: max-shm-memory
  type: string
- description: Maximum number of shared memory identifiers
  name: max-shm-ids
  type: integer
- description: Maximum number of message queue identifiers
  name: max-msg-ids
  type: integer
- description: Maximum number of semaphore identifiers
  name: max-sem-ids
  type: integer
- description: Current runtime state of the zone (read-only, not a configuration property)
  name: state
  type: string
- description: Kernel-assigned zone ID when the zone is running (read-only)
  name: id
  type: integer
- description: Automatic network interface resources providing network connectivity
  name: anet
  type: array
- description: ''
  name: capped-cpu
  type: object
- description: ''
  name: capped-memory
  type: object
- description: ''
  name: dedicated-cpu
  type: object
- description: ''
  name: virtual-cpu
  type: object
- description: Device resources made available to the zone
  name: device
  type: array
- description: File system mount resources
  name: fs
  type: array
- description: Network interface resources for shared-IP zones
  name: net
  type: array
- description: ZFS dataset resources delegated to the zone
  name: dataset
  type: array
- description: Resource control entries for the zone
  name: rctl
  type: array
- description: Generic attribute key-value pairs
  name: attr
  type: array
- description: Administrative access entries for zone delegation
  name: admin
  type: array
- description: ''
  name: rootzpool
  type: object
- description: Additional ZFS pools available to the zone
  name: zpool
  type: array
- description: SMF service dependencies required before zone boot
  name: smf-dependency
  type: array
- description: ''
  name: verified-boot
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-configuration-schema.json
slug: solaris-zone-configuration
source_filename: solaris-zone-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone-configuration.json\",\n  \"title\": \"Oracle Solaris Zone Configuration\",\n  \"description\": \"Represents a complete Solaris zone configuration including global properties, resource assignments, and networking for non-global zones managed through zonecfg(8) and the RAD zonemgr module.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"brand\", \"zonepath\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique name identifying the zone on the system\",\n      \"minLength\": 1,\n      \"maxLength\": 64,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9._-]*$\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Universally unique identifier assigned to the zone\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone\
  \ brand determining the runtime environment and kernel behavior\",\n      \"enum\": [\"solaris\", \"solaris10\", \"solaris-kz\", \"labeled\"]\n    },\n    \"zonepath\": {\n      \"type\": \"string\",\n      \"description\": \"File system path for the zone root directory\",\n      \"examples\": [\"/system/zones/testzone1\"]\n    },\n    \"autoboot\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the zone should automatically boot when the global zone boots\",\n      \"default\": false\n    },\n    \"autoshutdown\": {\n      \"type\": \"string\",\n      \"description\": \"Action to take when the global zone is shut down\",\n      \"enum\": [\"shutdown\", \"suspend\"],\n      \"default\": \"shutdown\"\n    },\n    \"bootargs\": {\n      \"type\": \"string\",\n      \"description\": \"Boot arguments passed to the zone at boot time\"\n    },\n    \"file-mac-profile\": {\n      \"type\": \"string\",\n      \"description\": \"File MAC policy profile for mandatory access control\"\
  \n    },\n    \"hostid\": {\n      \"type\": \"string\",\n      \"description\": \"Emulated host identifier for the zone\",\n      \"pattern\": \"^[0-9a-fA-F]{1,8}$\"\n    },\n    \"ip-type\": {\n      \"type\": \"string\",\n      \"description\": \"IP stack type for the zone\",\n      \"enum\": [\"exclusive\", \"shared\"],\n      \"default\": \"exclusive\"\n    },\n    \"limitpriv\": {\n      \"type\": \"string\",\n      \"description\": \"Comma-separated list of privileges for the zone\",\n      \"examples\": [\"default,dtrace_user,dtrace_proc\"]\n    },\n    \"scheduling-class\": {\n      \"type\": \"string\",\n      \"description\": \"Default scheduling class for processes in the zone\",\n      \"examples\": [\"FSS\", \"TS\"]\n    },\n    \"max-lwps\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of lightweight processes allowed in the zone\",\n      \"minimum\": 0\n    },\n    \"max-processes\": {\n      \"type\": \"integer\",\n      \"description\": \"\
  Maximum number of processes allowed in the zone\",\n      \"minimum\": 0\n    },\n    \"max-shm-memory\": {\n      \"type\": \"string\",\n      \"description\": \"Maximum shared memory allowed for the zone\",\n      \"examples\": [\"256m\", \"1g\"]\n    },\n    \"max-shm-ids\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of shared memory identifiers\",\n      \"minimum\": 0\n    },\n    \"max-msg-ids\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of message queue identifiers\",\n      \"minimum\": 0\n    },\n    \"max-sem-ids\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of semaphore identifiers\",\n      \"minimum\": 0\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current runtime state of the zone (read-only, not a configuration property)\",\n      \"enum\": [\"configured\", \"incomplete\", \"installed\", \"ready\", \"running\", \"shutting_down\", \"down\"],\n   \
  \   \"readOnly\": true\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Kernel-assigned zone ID when the zone is running (read-only)\",\n      \"readOnly\": true\n    },\n    \"anet\": {\n      \"type\": \"array\",\n      \"description\": \"Automatic network interface resources providing network connectivity\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AnetResource\"\n      }\n    },\n    \"capped-cpu\": {\n      \"$ref\": \"#/$defs/CappedCpuResource\"\n    },\n    \"capped-memory\": {\n      \"$ref\": \"#/$defs/CappedMemoryResource\"\n    },\n    \"dedicated-cpu\": {\n      \"$ref\": \"#/$defs/DedicatedCpuResource\"\n    },\n    \"virtual-cpu\": {\n      \"$ref\": \"#/$defs/VirtualCpuResource\"\n    },\n    \"device\": {\n      \"type\": \"array\",\n      \"description\": \"Device resources made available to the zone\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DeviceResource\"\n      }\n    },\n    \"fs\": {\n      \"type\": \"array\",\n  \
  \    \"description\": \"File system mount resources\",\n      \"items\": {\n        \"$ref\": \"#/$defs/FsResource\"\n      }\n    },\n    \"net\": {\n      \"type\": \"array\",\n      \"description\": \"Network interface resources for shared-IP zones\",\n      \"items\": {\n        \"$ref\": \"#/$defs/NetResource\"\n      }\n    },\n    \"dataset\": {\n      \"type\": \"array\",\n      \"description\": \"ZFS dataset resources delegated to the zone\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DatasetResource\"\n      }\n    },\n    \"rctl\": {\n      \"type\": \"array\",\n      \"description\": \"Resource control entries for the zone\",\n      \"items\": {\n        \"$ref\": \"#/$defs/RctlResource\"\n      }\n    },\n    \"attr\": {\n      \"type\": \"array\",\n      \"description\": \"Generic attribute key-value pairs\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AttrResource\"\n      }\n    },\n    \"admin\": {\n      \"type\": \"array\",\n      \"description\": \"Administrative\
  \ access entries for zone delegation\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AdminResource\"\n      }\n    },\n    \"rootzpool\": {\n      \"$ref\": \"#/$defs/RootzpoolResource\"\n    },\n    \"zpool\": {\n      \"type\": \"array\",\n      \"description\": \"Additional ZFS pools available to the zone\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ZpoolResource\"\n      }\n    },\n    \"smf-dependency\": {\n      \"type\": \"array\",\n      \"description\": \"SMF service dependencies required before zone boot\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SmfDependencyResource\"\n      }\n    },\n    \"verified-boot\": {\n      \"$ref\": \"#/$defs/VerifiedBootResource\"\n    }\n  },\n  \"$defs\": {\n    \"AnetResource\": {\n      \"type\": \"object\",\n      \"description\": \"Automatic network interface providing exclusive-IP networking for the zone\",\n      \"properties\": {\n        \"linkname\": {\n          \"type\": \"string\",\n          \"description\": \"\
  Name of the network link inside the zone\",\n          \"examples\": [\"net0\"]\n        },\n        \"lower-link\": {\n          \"type\": \"string\",\n          \"description\": \"Physical link over which the VNIC is created\",\n          \"examples\": [\"auto\", \"net0\"]\n        },\n        \"mac-address\": {\n          \"type\": \"string\",\n          \"description\": \"MAC address for the virtual NIC\",\n          \"examples\": [\"auto\", \"random\", \"02:08:20:12:34:56\"]\n        },\n        \"vlan-id\": {\n          \"type\": \"integer\",\n          \"description\": \"VLAN identifier for tagged traffic\",\n          \"minimum\": 0,\n          \"maximum\": 4094\n        },\n        \"mtu\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum transmission unit size\",\n          \"minimum\": 576,\n          \"maximum\": 9000\n        },\n        \"defrouter\": {\n          \"type\": \"string\",\n          \"description\": \"Default router IP address\",\n \
  \         \"examples\": [\"10.0.0.1\"]\n        },\n        \"allowed-address\": {\n          \"type\": \"string\",\n          \"description\": \"IP address or CIDR permitted on this interface\",\n          \"examples\": [\"10.0.0.100/24\"]\n        },\n        \"configure-allowed-address\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to automatically configure the allowed address on the interface\",\n          \"default\": true\n        },\n        \"link-protection\": {\n          \"type\": \"string\",\n          \"description\": \"Link protection mode to prevent spoofing\",\n          \"examples\": [\"mac-nospoof,ip-nospoof\"]\n        },\n        \"auto-mac-address\": {\n          \"type\": \"string\",\n          \"description\": \"Automatic MAC address assignment policy\"\n        },\n        \"mac-prefix\": {\n          \"type\": \"string\",\n          \"description\": \"MAC address prefix for auto-assigned addresses\"\n        },\n        \"mac-slot\"\
  : {\n          \"type\": \"integer\",\n          \"description\": \"MAC address slot number\"\n        },\n        \"vsi-typeid\": {\n          \"type\": \"integer\",\n          \"description\": \"VSI type identifier\"\n        },\n        \"vsi-typeidversion\": {\n          \"type\": \"integer\",\n          \"description\": \"VSI type identifier version\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Resource identifier\"\n        }\n      }\n    },\n    \"CappedCpuResource\": {\n      \"type\": \"object\",\n      \"description\": \"CPU cap limiting the total CPU time available to the zone\",\n      \"properties\": {\n        \"ncpus\": {\n          \"type\": \"number\",\n          \"description\": \"CPU cap expressed as a decimal number of CPUs (e.g., 1.5 = 150% of one CPU)\",\n          \"minimum\": 0,\n          \"examples\": [1.0, 2.5]\n        }\n      },\n      \"required\": [\"ncpus\"]\n    },\n    \"CappedMemoryResource\": {\n \
  \     \"type\": \"object\",\n      \"description\": \"Memory caps limiting physical and swap memory available to the zone\",\n      \"properties\": {\n        \"physical\": {\n          \"type\": \"string\",\n          \"description\": \"Physical memory cap\",\n          \"examples\": [\"2G\", \"512M\"]\n        },\n        \"swap\": {\n          \"type\": \"string\",\n          \"description\": \"Swap memory cap\",\n          \"examples\": [\"4G\", \"1G\"]\n        },\n        \"locked\": {\n          \"type\": \"string\",\n          \"description\": \"Locked memory cap\",\n          \"examples\": [\"512M\"]\n        }\n      }\n    },\n    \"DedicatedCpuResource\": {\n      \"type\": \"object\",\n      \"description\": \"Dedicated CPU resource guaranteeing exclusive CPU access\",\n      \"properties\": {\n        \"ncpus\": {\n          \"type\": \"string\",\n          \"description\": \"Number or range of CPUs dedicated to the zone\",\n          \"examples\": [\"2\", \"1-4\"]\n    \
  \    },\n        \"importance\": {\n          \"type\": \"integer\",\n          \"description\": \"Relative importance for CPU allocation when oversubscribed\",\n          \"minimum\": 1\n        }\n      },\n      \"required\": [\"ncpus\"]\n    },\n    \"VirtualCpuResource\": {\n      \"type\": \"object\",\n      \"description\": \"Virtual CPU resource for kernel zones (solaris-kz brand only)\",\n      \"properties\": {\n        \"ncpus\": {\n          \"type\": \"string\",\n          \"description\": \"Number or range of virtual CPUs\",\n          \"examples\": [\"4\", \"2-8\"]\n        }\n      },\n      \"required\": [\"ncpus\"]\n    },\n    \"DeviceResource\": {\n      \"type\": \"object\",\n      \"description\": \"Device resource allowing access to a host device from within the zone\",\n      \"properties\": {\n        \"match\": {\n          \"type\": \"string\",\n          \"description\": \"Device path pattern to match\",\n          \"examples\": [\"/dev/zvol/dsk/rpool/zvol1\"\
  ]\n        },\n        \"allow-partition\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to allow access to device partitions\"\n        },\n        \"allow-raw-io\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to allow raw I/O access to the device\"\n        },\n        \"storage\": {\n          \"type\": \"string\",\n          \"description\": \"Storage URI for the device\"\n        },\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Resource identifier\"\n        }\n      },\n      \"required\": [\"match\"]\n    },\n    \"FsResource\": {\n      \"type\": \"object\",\n      \"description\": \"File system mount providing host file system access within the zone\",\n      \"required\": [\"dir\", \"special\", \"type\"],\n      \"properties\": {\n        \"dir\": {\n          \"type\": \"string\",\n          \"description\": \"Mount point directory inside the zone\",\n          \"examples\": [\"/opt/shared\"\
  ]\n        },\n        \"special\": {\n          \"type\": \"string\",\n          \"description\": \"Source file system path or device on the host\",\n          \"examples\": [\"/export/shared\"]\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"File system type\",\n          \"enum\": [\"lofs\", \"hsfs\", \"nfs\", \"tmpfs\", \"ufs\", \"zfs\"]\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Mount options\",\n          \"examples\": [[\"ro\", \"nosuid\"]]\n        },\n        \"raw\": {\n          \"type\": \"string\",\n          \"description\": \"Raw device path for fsck operations\"\n        }\n      }\n    },\n    \"NetResource\": {\n      \"type\": \"object\",\n      \"description\": \"Network interface resource for shared-IP zones\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"IP address for the network interface\",\n          \"examples\": [\"10.0.0.100/24\"]\n        },\n        \"physical\": {\n          \"type\": \"string\",\n          \"description\": \"Physical network interface name\",\n          \"examples\": [\"net0\"]\n        },\n        \"defrouter\": {\n          \"type\": \"string\",\n          \"description\": \"Default router IP address\"\n        }\n      },\n      \"required\": [\"address\", \"physical\"]\n    },\n    \"DatasetResource\": {\n      \"type\": \"object\",\n      \"description\": \"ZFS dataset delegated to the zone for direct management\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"ZFS dataset name\",\n          \"examples\": [\"rpool/export/zones/testzone1/data\"]\n        },\n        \"alias\": {\n          \"type\": \"string\",\n          \"description\": \"Alias name for the dataset inside the zone\"\n        }\n      },\n      \"\
  required\": [\"name\"]\n    },\n    \"RctlResource\": {\n      \"type\": \"object\",\n      \"description\": \"Resource control entry limiting system resource usage within the zone\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Resource control name\",\n          \"examples\": [\"zone.max-lwps\", \"zone.max-shm-memory\", \"zone.cpu-shares\"]\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Resource control value in the form (priv=X,limit=Y,action=Z)\",\n          \"examples\": [\"(priv=privileged,limit=1000,action=deny)\"]\n        }\n      },\n      \"required\": [\"name\", \"value\"]\n    },\n    \"AttrResource\": {\n      \"type\": \"object\",\n      \"description\": \"Generic attribute resource for custom zone configuration properties\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Attribute name\"\n       \
  \ },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Attribute data type\",\n          \"enum\": [\"string\", \"int\", \"uint\", \"boolean\"]\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"Attribute value\"\n        }\n      },\n      \"required\": [\"name\", \"type\", \"value\"]\n    },\n    \"AdminResource\": {\n      \"type\": \"object\",\n      \"description\": \"Administrative access entry defining who can manage the zone\",\n      \"properties\": {\n        \"user\": {\n          \"type\": \"string\",\n          \"description\": \"User or role name granted administrative access\",\n          \"examples\": [\"zoneadm\"]\n        },\n        \"auths\": {\n          \"type\": \"string\",\n          \"description\": \"Comma-separated list of authorizations granted\",\n          \"examples\": [\"login,manage,config\"]\n        }\n      },\n      \"required\": [\"user\", \"auths\"]\n    },\n    \"RootzpoolResource\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Root ZFS pool configuration for the zone (solaris and solaris10 brands only)\",\n      \"properties\": {\n        \"storage\": {\n          \"type\": \"string\",\n          \"description\": \"Storage URI for the root zpool\"\n        }\n      }\n    },\n    \"ZpoolResource\": {\n      \"type\": \"object\",\n      \"description\": \"Additional ZFS pool available within the zone\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the ZFS pool\"\n        },\n        \"storage\": {\n          \"type\": \"string\",\n          \"description\": \"Storage URI for the pool\"\n        }\n      },\n      \"required\": [\"name\"]\n    },\n    \"SmfDependencyResource\": {\n      \"type\": \"object\",\n      \"description\": \"SMF service dependency that must be satisfied before zone boot\",\n      \"properties\": {\n        \"fmri\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"Fault Management Resource Identifier of the SMF service\",\n          \"examples\": [\"svc:/network/physical:default\"]\n        },\n        \"grouping\": {\n          \"type\": \"string\",\n          \"description\": \"Dependency grouping type\",\n          \"enum\": [\"require_all\", \"require_any\", \"optional_all\", \"exclude_all\"]\n        }\n      },\n      \"required\": [\"fmri\"]\n    },\n    \"VerifiedBootResource\": {\n      \"type\": \"object\",\n      \"description\": \"Verified boot settings for kernel zone security (solaris-kz brand only)\",\n      \"properties\": {\n        \"firmware\": {\n          \"type\": \"string\",\n          \"description\": \"Firmware image path for verified boot\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-configuration-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: Oracle Solaris Zone Configuration
---
