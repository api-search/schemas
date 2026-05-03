---
description: JSON Schema for the OCI Runtime Specification container configuration (config.json). This file defines the container's execution environment, process, mounts, namespaces, cgroups, and security settings as required by runc and the OCI Runtime Spec.
layout: schema
name: OCI Runtime Container Configuration
properties_list:
- description: The version of the OCI Runtime Specification with which the bundle complies.
  name: ociVersion
  type: string
- description: The container process configuration.
  name: process
  type: object
- description: The root filesystem configuration.
  name: root
  type: object
- description: The hostname to set inside the container.
  name: hostname
  type: string
- description: Additional filesystem mounts for the container.
  name: mounts
  type: array
- description: Linux-specific configuration for the container.
  name: linux
  type: object
- description: Lifecycle hooks for the container.
  name: hooks
  type: object
- description: Arbitrary metadata for the container as key-value string pairs.
  name: annotations
  type: object
provider_name: Runc
provider_slug: runc
schema_file: json-schema/runc-container-config-schema.json
slug: runc-container-config
source_filename: runc-container-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/runc/blob/main/json-schema/runc-container-config-schema.json\",\n  \"title\": \"OCI Runtime Container Configuration\",\n  \"description\": \"JSON Schema for the OCI Runtime Specification container configuration (config.json). This file defines the container's execution environment, process, mounts, namespaces, cgroups, and security settings as required by runc and the OCI Runtime Spec.\",\n  \"type\": \"object\",\n  \"required\": [\"ociVersion\", \"process\", \"root\"],\n  \"properties\": {\n    \"ociVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the OCI Runtime Specification with which the bundle complies.\"\n    },\n    \"process\": {\n      \"type\": \"object\",\n      \"description\": \"The container process configuration.\",\n      \"required\": [\"args\"],\n      \"properties\": {\n        \"terminal\": {\n          \"\
  type\": \"boolean\",\n          \"description\": \"Whether a terminal is attached to the process.\"\n        },\n        \"user\": {\n          \"type\": \"object\",\n          \"description\": \"The user executing the process.\",\n          \"properties\": {\n            \"uid\": { \"type\": \"integer\", \"description\": \"User ID.\" },\n            \"gid\": { \"type\": \"integer\", \"description\": \"Group ID.\" },\n            \"additionalGids\": {\n              \"type\": \"array\",\n              \"items\": { \"type\": \"integer\" },\n              \"description\": \"Additional group IDs.\"\n            }\n          }\n        },\n        \"args\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"The command to run with arguments. args[0] is the executable path.\"\n        },\n        \"env\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Environment variables\
  \ for the container process in KEY=value format.\"\n        },\n        \"cwd\": {\n          \"type\": \"string\",\n          \"description\": \"The working directory of the container process.\"\n        },\n        \"capabilities\": {\n          \"type\": \"object\",\n          \"description\": \"Linux capabilities for the process.\",\n          \"properties\": {\n            \"bounding\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n            \"effective\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n            \"inheritable\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n            \"permitted\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n            \"ambient\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n          }\n        },\n        \"noNewPrivileges\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the process cannot gain additional privileges via setuid/setgid.\"\
  \n        }\n      }\n    },\n    \"root\": {\n      \"type\": \"object\",\n      \"description\": \"The root filesystem configuration.\",\n      \"required\": [\"path\"],\n      \"properties\": {\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"Path to the root filesystem directory (absolute or relative to bundle).\"\n        },\n        \"readonly\": {\n          \"type\": \"boolean\",\n          \"description\": \"If true, the root filesystem is mounted read-only.\"\n        }\n      }\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname to set inside the container.\"\n    },\n    \"mounts\": {\n      \"type\": \"array\",\n      \"description\": \"Additional filesystem mounts for the container.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\"destination\"],\n        \"properties\": {\n          \"destination\": { \"type\": \"string\", \"description\": \"Destination path inside\
  \ the container.\" },\n          \"type\": { \"type\": \"string\", \"description\": \"Filesystem type (e.g., proc, tmpfs, bind).\" },\n          \"source\": { \"type\": \"string\", \"description\": \"Source path on the host.\" },\n          \"options\": {\n            \"type\": \"array\",\n            \"items\": { \"type\": \"string\" },\n            \"description\": \"Mount options (e.g., rbind, ro, nosuid).\"\n          }\n        }\n      }\n    },\n    \"linux\": {\n      \"type\": \"object\",\n      \"description\": \"Linux-specific configuration for the container.\",\n      \"properties\": {\n        \"namespaces\": {\n          \"type\": \"array\",\n          \"description\": \"Linux namespaces for the container.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"required\": [\"type\"],\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"pid\", \"network\", \"mount\", \"ipc\", \"\
  uts\", \"user\", \"cgroup\"],\n                \"description\": \"The type of namespace.\"\n              },\n              \"path\": {\n                \"type\": \"string\",\n                \"description\": \"Path to the namespace file (for sharing an existing namespace).\"\n              }\n            }\n          }\n        },\n        \"resources\": {\n          \"type\": \"object\",\n          \"description\": \"Cgroup resource limits for the container.\",\n          \"properties\": {\n            \"memory\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"limit\": { \"type\": \"integer\", \"description\": \"Memory limit in bytes.\" },\n                \"swap\": { \"type\": \"integer\", \"description\": \"Memory + swap limit in bytes.\" },\n                \"reservation\": { \"type\": \"integer\", \"description\": \"Memory soft limit in bytes.\" }\n              }\n            },\n            \"cpu\": {\n              \"type\": \"object\"\
  ,\n              \"properties\": {\n                \"shares\": { \"type\": \"integer\", \"description\": \"CPU shares (relative weight).\" },\n                \"quota\": { \"type\": \"integer\", \"description\": \"CPU CFS quota in microseconds.\" },\n                \"period\": { \"type\": \"integer\", \"description\": \"CPU CFS period in microseconds.\" }\n              }\n            }\n          }\n        },\n        \"seccomp\": {\n          \"type\": \"object\",\n          \"description\": \"Seccomp profile for system call filtering.\",\n          \"properties\": {\n            \"defaultAction\": { \"type\": \"string\", \"description\": \"Default action for unmatched syscalls.\" },\n            \"syscalls\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"names\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n                  \"action\": { \"type\":\
  \ \"string\" }\n                }\n              }\n            }\n          }\n        },\n        \"maskedPaths\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Paths that should be masked inside the container.\"\n        },\n        \"readonlyPaths\": {\n          \"type\": \"array\",\n          \"items\": { \"type\": \"string\" },\n          \"description\": \"Paths that should be read-only inside the container.\"\n        }\n      }\n    },\n    \"hooks\": {\n      \"type\": \"object\",\n      \"description\": \"Lifecycle hooks for the container.\",\n      \"properties\": {\n        \"prestart\": { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/Hook\" } },\n        \"createRuntime\": { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/Hook\" } },\n        \"createContainer\": { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/Hook\" } },\n        \"startContainer\": { \"type\": \"array\", \"items\":\
  \ { \"$ref\": \"#/$defs/Hook\" } },\n        \"poststart\": { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/Hook\" } },\n        \"poststop\": { \"type\": \"array\", \"items\": { \"$ref\": \"#/$defs/Hook\" } }\n      }\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"Arbitrary metadata for the container as key-value string pairs.\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    }\n  },\n  \"$defs\": {\n    \"Hook\": {\n      \"type\": \"object\",\n      \"required\": [\"path\"],\n      \"properties\": {\n        \"path\": { \"type\": \"string\", \"description\": \"Absolute path to the hook executable.\" },\n        \"args\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"env\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"timeout\": { \"type\": \"integer\", \"description\": \"Timeout in seconds.\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/runc/refs/heads/main/json-schema/runc-container-config-schema.json
tags:
- Container Runtime
- Containers
- Linux
- OCI
- Open Source
- CNCF
- Open Container Initiative
- Cloud Native
title: OCI Runtime Container Configuration
---
