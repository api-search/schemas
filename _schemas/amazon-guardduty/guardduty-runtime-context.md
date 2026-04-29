---
description: Additional information about the suspicious activity.
layout: schema
name: RuntimeContext
properties_list:
- description: ''
  name: ModifyingProcess
  type: object
- description: ''
  name: ModifiedAt
  type: object
- description: ''
  name: ScriptPath
  type: object
- description: ''
  name: LibraryPath
  type: object
- description: ''
  name: LdPreloadValue
  type: object
- description: ''
  name: SocketPath
  type: object
- description: ''
  name: RuncBinaryPath
  type: object
- description: ''
  name: ReleaseAgentPath
  type: object
- description: ''
  name: MountSource
  type: object
- description: ''
  name: MountTarget
  type: object
- description: ''
  name: FileSystemType
  type: object
- description: ''
  name: Flags
  type: object
- description: ''
  name: ModuleName
  type: object
- description: ''
  name: ModuleFilePath
  type: object
- description: ''
  name: ModuleSha256
  type: object
- description: ''
  name: ShellHistoryFilePath
  type: object
- description: ''
  name: TargetProcess
  type: object
- description: ''
  name: AddressFamily
  type: object
- description: ''
  name: IanaProtocolNumber
  type: object
- description: ''
  name: MemoryRegions
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-runtime-context-schema.json
slug: guardduty-runtime-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-runtime-context-schema.json\",\n  \"title\": \"RuntimeContext\",\n  \"description\": \"Additional information about the suspicious activity.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ModifyingProcess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProcessDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"modifyingProcess\"\n          },\n          \"description\": \"Information about the process that modified the current process. This is available for multiple finding types.\"\n        }\n      ]\n    },\n    \"ModifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"modifiedAt\"\n          },\n        \
  \  \"description\": \"The timestamp at which the process modified the current process. The timestamp is in UTC date string format.\"\n        }\n      ]\n    },\n    \"ScriptPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"scriptPath\"\n          },\n          \"description\": \"The path to the script that was executed.\"\n        }\n      ]\n    },\n    \"LibraryPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"libraryPath\"\n          },\n          \"description\": \"The path to the new library that was loaded.\"\n        }\n      ]\n    },\n    \"LdPreloadValue\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ldPreloadValue\"\n          },\n        \
  \  \"description\": \"The value of the LD_PRELOAD environment variable.\"\n        }\n      ]\n    },\n    \"SocketPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"socketPath\"\n          },\n          \"description\": \"The path to the docket socket that was accessed.\"\n        }\n      ]\n    },\n    \"RuncBinaryPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"runcBinaryPath\"\n          },\n          \"description\": \"The path to the leveraged <code>runc</code> implementation.\"\n        }\n      ]\n    },\n    \"ReleaseAgentPath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"releaseAgentPath\"\n          },\n          \"description\": \"The path\
  \ in the container that modified the release agent file.\"\n        }\n      ]\n    },\n    \"MountSource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mountSource\"\n          },\n          \"description\": \"The path on the host that is mounted by the container.\"\n        }\n      ]\n    },\n    \"MountTarget\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mountTarget\"\n          },\n          \"description\": \"The path in the container that is mapped to the host directory.\"\n        }\n      ]\n    },\n    \"FileSystemType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fileSystemType\"\n          },\n          \"description\": \"Represents the type\
  \ of mounted fileSystem.\"\n        }\n      ]\n    },\n    \"Flags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlagsList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"flags\"\n          },\n          \"description\": \"Represents options that control the behavior of a runtime operation or action. For example, a filesystem mount operation may contain a read-only flag.\"\n        }\n      ]\n    },\n    \"ModuleName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"moduleName\"\n          },\n          \"description\": \"The name of the module loaded into the kernel.\"\n        }\n      ]\n    },\n    \"ModuleFilePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"moduleFilePath\"\n          },\n          \"\
  description\": \"The path to the module loaded into the kernel.\"\n        }\n      ]\n    },\n    \"ModuleSha256\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"moduleSha256\"\n          },\n          \"description\": \"The <code>SHA256</code> hash of the module.\"\n        }\n      ]\n    },\n    \"ShellHistoryFilePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shellHistoryFilePath\"\n          },\n          \"description\": \"The path to the modified shell history file.\"\n        }\n      ]\n    },\n    \"TargetProcess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProcessDetails\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetProcess\"\n          },\n          \"description\": \"Information about\
  \ the process that had its memory overwritten by the current process.\"\n        }\n      ]\n    },\n    \"AddressFamily\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"addressFamily\"\n          },\n          \"description\": \"Represents the communication protocol associated with the address. For example, the address family <code>AF_INET</code> is used for IP version of 4 protocol.\"\n        }\n      ]\n    },\n    \"IanaProtocolNumber\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ianaProtocolNumber\"\n          },\n          \"description\": \"Specifies a particular protocol within the address family. Usually there is a single protocol in address families. For example, the address family <code>AF_INET</code> only has the IP protocol.\"\n        }\n      ]\n   \
  \ },\n    \"MemoryRegions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MemoryRegionsList\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"memoryRegions\"\n          },\n          \"description\": \"Specifies the Region of a process's address space such as stack and heap.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-runtime-context-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RuntimeContext
---
