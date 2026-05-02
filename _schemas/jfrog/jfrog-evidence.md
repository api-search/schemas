---
description: Represents an evidence attestation in the JFrog Platform, providing a cryptographically signed record of an external process performed on a software artifact, build, package, or release bundle. Evidence is stored as in-toto statements wrapped in DSSE (Dead Simple Signing Envelope) format.
layout: schema
name: JFrog Evidence
properties_list:
- description: Unique evidence record identifier
  name: id
  type: string
- description: Type of the subject the evidence is attached to
  name: subject_type
  type: string
- description: Subject identification details
  name: subject
  type: object
- description: URI identifying the predicate type (in-toto attestation type)
  name: predicate_type
  type: string
- description: The evidence predicate content conforming to the predicate_type schema
  name: predicate
  type: object
- description: Path to the DSSE signed envelope file stored in Artifactory
  name: dsse_envelope_path
  type: string
- description: Cryptographic algorithm used for signing the evidence
  name: signature_algorithm
  type: string
- description: Alias of the public key registered for signature verification
  name: key_alias
  type: string
- description: Whether the evidence signature has been successfully verified
  name: verified
  type: boolean
- description: Timestamp when the evidence was created
  name: created
  type: string
- description: User or service that created the evidence
  name: created_by
  type: string
provider_name: JFrog
provider_slug: jfrog
schema_file: json-schema/jfrog-evidence-schema.json
slug: jfrog-evidence
source_filename: jfrog-evidence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://jfrog.com/schemas/evidence\",\n  \"title\": \"JFrog Evidence\",\n  \"description\": \"Represents an evidence attestation in the JFrog Platform, providing a cryptographically signed record of an external process performed on a software artifact, build, package, or release bundle. Evidence is stored as in-toto statements wrapped in DSSE (Dead Simple Signing Envelope) format.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique evidence record identifier\"\n    },\n    \"subject_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the subject the evidence is attached to\",\n      \"enum\": [\n        \"artifact\",\n        \"build\",\n        \"package\",\n        \"release_bundle\"\n      ]\n    },\n    \"subject\": {\n      \"type\": \"object\",\n      \"description\": \"Subject identification details\"\
  ,\n      \"properties\": {\n        \"repo_path\": {\n          \"type\": \"string\",\n          \"description\": \"Artifact repository path\"\n        },\n        \"sha256\": {\n          \"type\": \"string\",\n          \"description\": \"SHA-256 digest of the subject artifact\"\n        },\n        \"build_name\": {\n          \"type\": \"string\"\n        },\n        \"build_number\": {\n          \"type\": \"string\"\n        },\n        \"package_name\": {\n          \"type\": \"string\"\n        },\n        \"package_version\": {\n          \"type\": \"string\"\n        },\n        \"repo_key\": {\n          \"type\": \"string\"\n        },\n        \"release_bundle_name\": {\n          \"type\": \"string\"\n        },\n        \"release_bundle_version\": {\n          \"type\": \"string\"\n        },\n        \"project\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"predicate_type\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"URI identifying the predicate type (in-toto attestation type)\",\n      \"examples\": [\n        \"https://in-toto.io/attestation/vulns\",\n        \"https://slsa.dev/provenance/v1\",\n        \"https://in-toto.io/attestation/test-result/v0.1\"\n      ]\n    },\n    \"predicate\": {\n      \"type\": \"object\",\n      \"additionalProperties\": true,\n      \"description\": \"The evidence predicate content conforming to the predicate_type schema\"\n    },\n    \"dsse_envelope_path\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the DSSE signed envelope file stored in Artifactory\"\n    },\n    \"signature_algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"Cryptographic algorithm used for signing the evidence\",\n      \"enum\": [\n        \"ECDSA\",\n        \"RSA\",\n        \"ED25519\"\n      ]\n    },\n    \"key_alias\": {\n      \"type\": \"string\",\n      \"description\": \"Alias of the public key registered for signature verification\"\n\
  \    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the evidence signature has been successfully verified\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the evidence was created\"\n    },\n    \"created_by\": {\n      \"type\": \"string\",\n      \"description\": \"User or service that created the evidence\"\n    }\n  },\n  \"required\": [\n    \"subject_type\",\n    \"subject\",\n    \"predicate_type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jfrog/refs/heads/main/json-schema/jfrog-evidence-schema.json
tags:
- Artifactory
- CI/CD
- Container Registry
- DevOps
- MLOps
- Package Management
- Security
- Software Supply Chain
title: JFrog Evidence
---
