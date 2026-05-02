---
description: Schema for the in-toto Link metadata document, which records what actually happened at a single step in the software supply chain. A link captures the command that was run, the materials consumed (files present before the command), and the products produced (files present after the command), each identified by cryptographic hash. Links are signed by the functionary who performed the step.
layout: schema
name: in-toto Link
properties_list:
- description: Identifies this metadata document as an in-toto link.
  name: _type
  type: string
- description: Name of the step this link corresponds to. Must match a step name defined in the layout.
  name: name
  type: string
- description: The command that was executed to perform this step, represented as an array of argument tokens.
  name: command
  type: array
- description: Artifact dictionary for files present before the step was executed. Keys are file paths; values are hash objects mapping algorithm name to hex digest.
  name: materials
  type: object
- description: Artifact dictionary for files present after the step was executed. Keys are file paths; values are hash objects mapping algorithm name to hex digest.
  name: products
  type: object
- description: Incidental outputs from the step execution, such as stdout, stderr, and return value. These are recorded for auditability but not used in artifact rule evaluation.
  name: byproducts
  type: object
- description: Additional environment information at the time the step was performed. May include variables, working directory, or platform details for auditability.
  name: environment
  type: object
provider_name: In-Toto
provider_slug: in-toto
schema_file: json-schema/in-toto-link-schema.json
slug: in-toto-link
source_filename: in-toto-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://in-toto.io/schemas/v1/link.json\",\n  \"title\": \"in-toto Link\",\n  \"description\": \"Schema for the in-toto Link metadata document, which records what actually happened at a single step in the software supply chain. A link captures the command that was run, the materials consumed (files present before the command), and the products produced (files present after the command), each identified by cryptographic hash. Links are signed by the functionary who performed the step.\",\n  \"type\": \"object\",\n  \"required\": [\"_type\", \"name\", \"materials\", \"products\", \"command\", \"byproducts\", \"environment\"],\n  \"properties\": {\n    \"_type\": {\n      \"type\": \"string\",\n      \"const\": \"link\",\n      \"description\": \"Identifies this metadata document as an in-toto link.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the step\
  \ this link corresponds to. Must match a step name defined in the layout.\"\n    },\n    \"command\": {\n      \"type\": \"array\",\n      \"description\": \"The command that was executed to perform this step, represented as an array of argument tokens.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"materials\": {\n      \"type\": \"object\",\n      \"description\": \"Artifact dictionary for files present before the step was executed. Keys are file paths; values are hash objects mapping algorithm name to hex digest.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Hashes\"\n      }\n    },\n    \"products\": {\n      \"type\": \"object\",\n      \"description\": \"Artifact dictionary for files present after the step was executed. Keys are file paths; values are hash objects mapping algorithm name to hex digest.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Hashes\"\n      }\n    },\n    \"byproducts\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Incidental outputs from the step execution, such as stdout, stderr, and return value. These are recorded for auditability but not used in artifact rule evaluation.\",\n      \"properties\": {\n        \"stdout\": {\n          \"type\": \"string\",\n          \"description\": \"Standard output captured from the step command.\"\n        },\n        \"stderr\": {\n          \"type\": \"string\",\n          \"description\": \"Standard error output captured from the step command.\"\n        },\n        \"return-value\": {\n          \"type\": \"integer\",\n          \"description\": \"Exit code returned by the step command.\"\n        }\n      }\n    },\n    \"environment\": {\n      \"type\": \"object\",\n      \"description\": \"Additional environment information at the time the step was performed. May include variables, working directory, or platform details for auditability.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"$defs\": {\n \
  \   \"Hashes\": {\n      \"type\": \"object\",\n      \"description\": \"A map of cryptographic hash algorithm names to their corresponding hex-encoded digest values for a single artifact.\",\n      \"properties\": {\n        \"sha256\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{64}$\",\n          \"description\": \"SHA-256 hex digest of the artifact.\"\n        },\n        \"sha512\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{128}$\",\n          \"description\": \"SHA-512 hex digest of the artifact.\"\n        },\n        \"sha3_256\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[a-fA-F0-9]{64}$\",\n          \"description\": \"SHA3-256 hex digest of the artifact.\"\n        }\n      },\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"description\": \"Hex-encoded digest for an alternate hash algorithm.\"\n      },\n      \"minProperties\": 1\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/in-toto/refs/heads/main/json-schema/in-toto-link-schema.json
tags:
- Cloud Native
- Graduated
- Security
- Software Integrity
- Supply Chain Security
- Verification
title: in-toto Link
---
