---
description: Schema for The Update Framework (TUF) snapshot metadata document (snapshot.json). The snapshot metadata lists the current version numbers and optional hashes of all targets metadata files in the repository, including the top-level targets.json and all delegated targets metadata. Clients use the snapshot to ensure they have a consistent, atomic view of all metadata and to prevent mix-and-match attacks where an attacker combines metadata from different repository states.
layout: schema
name: TUF Snapshot Metadata
properties_list:
- description: ''
  name: signed
  type: object
- description: List of cryptographic signatures over the canonical JSON encoding of the signed field, produced by keys authorized for the snapshot role.
  name: signatures
  type: array
provider_name: The Update Framework (TUF)
provider_slug: tuf
schema_file: json-schema/tuf-snapshot-metadata-schema.json
slug: tuf-snapshot-metadata
source_filename: tuf-snapshot-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://theupdateframework.io/schemas/snapshot-metadata.json\",\n  \"title\": \"TUF Snapshot Metadata\",\n  \"description\": \"Schema for The Update Framework (TUF) snapshot metadata document (snapshot.json). The snapshot metadata lists the current version numbers and optional hashes of all targets metadata files in the repository, including the top-level targets.json and all delegated targets metadata. Clients use the snapshot to ensure they have a consistent, atomic view of all metadata and to prevent mix-and-match attacks where an attacker combines metadata from different repository states.\",\n  \"type\": \"object\",\n  \"required\": [\"signed\", \"signatures\"],\n  \"properties\": {\n    \"signed\": {\n      \"$ref\": \"#/$defs/SnapshotSigned\"\n    },\n    \"signatures\": {\n      \"type\": \"array\",\n      \"description\": \"List of cryptographic signatures over the canonical JSON encoding\
  \ of the signed field, produced by keys authorized for the snapshot role.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Signature\"\n      },\n      \"minItems\": 1\n    }\n  },\n  \"$defs\": {\n    \"SnapshotSigned\": {\n      \"type\": \"object\",\n      \"description\": \"The signed portion of snapshot metadata listing the current versions of all targets metadata files.\",\n      \"required\": [\"_type\", \"spec_version\", \"version\", \"expires\", \"meta\"],\n      \"properties\": {\n        \"_type\": {\n          \"type\": \"string\",\n          \"description\": \"Type identifier for this metadata document.\",\n          \"const\": \"snapshot\"\n        },\n        \"spec_version\": {\n          \"type\": \"string\",\n          \"description\": \"Version of the TUF specification this metadata conforms to.\",\n          \"pattern\": \"^\\\\d+\\\\.\\\\d+\\\\.\\\\d+$\",\n          \"examples\": [\"1.0.0\"]\n        },\n        \"version\": {\n          \"type\": \"integer\",\n\
  \          \"description\": \"Monotonically increasing version number for this snapshot metadata. Clients reject older versions to prevent rollback attacks.\",\n          \"minimum\": 1\n        },\n        \"expires\": {\n          \"type\": \"string\",\n          \"description\": \"ISO 8601 UTC datetime after which this snapshot metadata is expired.\",\n          \"format\": \"date-time\"\n        },\n        \"meta\": {\n          \"type\": \"object\",\n          \"description\": \"Map of metadata filename to MetaFile descriptor. Must include 'targets.json' and should include all delegated targets metadata files. Keys are filenames relative to the metadata directory.\",\n          \"required\": [\"targets.json\"],\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/MetaFile\"\n          },\n          \"examples\": [\n            {\n              \"targets.json\": { \"version\": 3 },\n              \"unclaimed.json\": { \"version\": 1, \"length\": 1234, \"hashes\"\
  : { \"sha256\": \"abc123...\" } }\n            }\n          ]\n        }\n      }\n    },\n    \"MetaFile\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a metadata file recorded in the snapshot, including its version number and optionally its length and hashes.\",\n      \"required\": [\"version\"],\n      \"properties\": {\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"Version number of the referenced metadata file. Clients use this to request the specific version and detect rollback attacks.\",\n          \"minimum\": 1\n        },\n        \"length\": {\n          \"type\": \"integer\",\n          \"description\": \"Length of the metadata file in bytes. Optional but recommended for detecting size-based attacks.\",\n          \"minimum\": 0\n        },\n        \"hashes\": {\n          \"type\": \"object\",\n          \"description\": \"Map of hash algorithm to hex-encoded hash digest of the metadata file content. Optional\
  \ but recommended for additional integrity protection.\",\n          \"properties\": {\n            \"sha256\": {\n              \"type\": \"string\",\n              \"description\": \"SHA-256 digest of the metadata file, hex-encoded.\",\n              \"pattern\": \"^[0-9a-f]{64}$\"\n            },\n            \"sha512\": {\n              \"type\": \"string\",\n              \"description\": \"SHA-512 digest of the metadata file, hex-encoded.\",\n              \"pattern\": \"^[0-9a-f]{128}$\"\n            }\n          },\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"description\": \"Hex-encoded hash digest for an additional algorithm.\"\n          }\n        }\n      }\n    },\n    \"Signature\": {\n      \"type\": \"object\",\n      \"description\": \"A cryptographic signature over the canonical JSON of the signed field.\",\n      \"required\": [\"keyid\", \"sig\"],\n      \"properties\": {\n        \"keyid\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"ID of the key that produced this signature.\",\n          \"pattern\": \"^[0-9a-f]{64}$\"\n        },\n        \"sig\": {\n          \"type\": \"string\",\n          \"description\": \"Hex-encoded signature bytes.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tuf/refs/heads/main/json-schema/tuf-snapshot-metadata-schema.json
tags:
- Cloud Native
- Graduated
- Security
- Software Updates
- Supply Chain
- Verification
title: TUF Snapshot Metadata
---
