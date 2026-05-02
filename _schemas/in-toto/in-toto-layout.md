---
description: Schema for the in-toto Layout metadata document, which defines the expected steps of a software supply chain, the authorized functionaries for each step, and the inspection rules used during verification. A signed Layout is the root of trust for an in-toto supply chain.
layout: schema
name: in-toto Layout
properties_list:
- description: Identifies this metadata document as an in-toto layout.
  name: _type
  type: string
- description: ISO 8601 date-time string after which this layout is considered expired and verification must fail.
  name: expires
  type: string
- description: Human-readable description of the software supply chain and the purpose of this layout.
  name: readme
  type: string
- description: Dictionary of public keys authorized to sign link metadata for steps in this layout. Keys are key IDs (fingerprints); values are key objects.
  name: keys
  type: object
- description: Ordered list of steps that must be performed in the software supply chain. Each step specifies who may perform it and what artifact rules must hold.
  name: steps
  type: array
- description: List of inspection commands to run during verification. Inspections compute link metadata locally and can apply artifact rules against the combined set of supply chain artifacts.
  name: inspect
  type: array
provider_name: In-Toto
provider_slug: in-toto
schema_file: json-schema/in-toto-layout-schema.json
slug: in-toto-layout
source_filename: in-toto-layout-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://in-toto.io/schemas/v1/layout.json\",\n  \"title\": \"in-toto Layout\",\n  \"description\": \"Schema for the in-toto Layout metadata document, which defines the expected steps of a software supply chain, the authorized functionaries for each step, and the inspection rules used during verification. A signed Layout is the root of trust for an in-toto supply chain.\",\n  \"type\": \"object\",\n  \"required\": [\"_type\", \"steps\", \"inspect\", \"keys\", \"expires\"],\n  \"properties\": {\n    \"_type\": {\n      \"type\": \"string\",\n      \"const\": \"layout\",\n      \"description\": \"Identifies this metadata document as an in-toto layout.\"\n    },\n    \"expires\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 date-time string after which this layout is considered expired and verification must fail.\"\n    },\n    \"readme\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Human-readable description of the software supply chain and the purpose of this layout.\"\n    },\n    \"keys\": {\n      \"type\": \"object\",\n      \"description\": \"Dictionary of public keys authorized to sign link metadata for steps in this layout. Keys are key IDs (fingerprints); values are key objects.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Key\"\n      }\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"description\": \"Ordered list of steps that must be performed in the software supply chain. Each step specifies who may perform it and what artifact rules must hold.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Step\"\n      }\n    },\n    \"inspect\": {\n      \"type\": \"array\",\n      \"description\": \"List of inspection commands to run during verification. Inspections compute link metadata locally and can apply artifact rules against the combined set of supply chain artifacts.\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/$defs/Inspection\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"Key\": {\n      \"type\": \"object\",\n      \"description\": \"A public key used to verify signatures on link metadata or on the layout itself.\",\n      \"required\": [\"keytype\", \"keyval\", \"scheme\"],\n      \"properties\": {\n        \"keytype\": {\n          \"type\": \"string\",\n          \"description\": \"Algorithm family for this key.\",\n          \"enum\": [\"rsa\", \"ed25519\", \"ecdsa\", \"rsa-pkcs1v15\"]\n        },\n        \"scheme\": {\n          \"type\": \"string\",\n          \"description\": \"Signing scheme used with this key, e.g. rsassa-pss-sha256 or ed25519.\"\n        },\n        \"keyid_hash_algorithms\": {\n          \"type\": \"array\",\n          \"description\": \"Hash algorithms used to compute the key ID.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"keyval\": {\n          \"type\": \"object\"\
  ,\n          \"description\": \"Key material. For asymmetric keys, contains a 'public' property with the PEM-encoded public key.\",\n          \"properties\": {\n            \"public\": {\n              \"type\": \"string\",\n              \"description\": \"PEM-encoded public key.\"\n            }\n          }\n        }\n      }\n    },\n    \"Step\": {\n      \"type\": \"object\",\n      \"description\": \"A single step in the software supply chain. Specifies who is authorized to perform the step and the artifact rules governing materials and products.\",\n      \"required\": [\"name\", \"pubkeys\", \"expected_materials\", \"expected_products\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Unique name identifying this step within the layout. Must match the name used in the corresponding link metadata.\"\n        },\n        \"pubkeys\": {\n          \"type\": \"array\",\n          \"description\": \"List of key IDs of\
  \ functionaries authorized to perform this step and sign its link metadata.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"expected_command\": {\n          \"type\": \"array\",\n          \"description\": \"Optional list of command tokens expected to be run for this step. Verification may warn if the actual command differs.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"expected_materials\": {\n          \"type\": \"array\",\n          \"description\": \"Artifact rules applied to materials recorded in this step's link metadata.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ArtifactRule\"\n          }\n        },\n        \"expected_products\": {\n          \"type\": \"array\",\n          \"description\": \"Artifact rules applied to products recorded in this step's link metadata.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ArtifactRule\"\n          }\n      \
  \  },\n        \"threshold\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"Minimum number of valid link metadata files required from different functionaries for this step to be considered complete.\",\n          \"default\": 1\n        }\n      }\n    },\n    \"Inspection\": {\n      \"type\": \"object\",\n      \"description\": \"A verification-time command that is run by the verifier to produce link metadata locally. Allows applying artifact rules over the final supply chain state.\",\n      \"required\": [\"name\", \"run\", \"expected_materials\", \"expected_products\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Unique name identifying this inspection within the layout.\"\n        },\n        \"run\": {\n          \"type\": \"array\",\n          \"description\": \"Command tokens to execute during the inspection phase of verification.\",\n          \"items\": {\n       \
  \     \"type\": \"string\"\n          }\n        },\n        \"expected_materials\": {\n          \"type\": \"array\",\n          \"description\": \"Artifact rules applied to materials recorded by this inspection.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ArtifactRule\"\n          }\n        },\n        \"expected_products\": {\n          \"type\": \"array\",\n          \"description\": \"Artifact rules applied to products recorded by this inspection.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/ArtifactRule\"\n          }\n        }\n      }\n    },\n    \"ArtifactRule\": {\n      \"type\": \"array\",\n      \"description\": \"A rule that constrains which artifacts (materials or products) are acceptable for a step. Rules are expressed as arrays of tokens following the in-toto artifact rule grammar, e.g. ['MATCH', 'foo', 'WITH', 'PRODUCTS', 'FROM', 'build'].\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 1\n    }\n \
  \ }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/in-toto/refs/heads/main/json-schema/in-toto-layout-schema.json
tags:
- Cloud Native
- Graduated
- Security
- Software Integrity
- Supply Chain Security
- Verification
title: in-toto Layout
---
