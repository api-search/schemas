---
description: A PEP 740 provenance object representing digital attestations for a Python package distribution file. Contains one or more attestation bundles verified by PyPI, along with the Trusted Publisher identity that produced them.
layout: schema
name: PyPI Provenance
properties_list:
- description: The provenance object format version. Currently always 1.
  name: version
  type: integer
- description: One or more attestation bundles, each containing the publisher identity and a set of attestations.
  name: attestation_bundles
  type: array
provider_name: PyPI
provider_slug: pypi
schema_file: json-schema/pypi-provenance-schema.json
slug: pypi-provenance
source_filename: pypi-provenance-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://pypi.org/schemas/pypi/provenance.json\",\n  \"title\": \"PyPI Provenance\",\n  \"description\": \"A PEP 740 provenance object representing digital attestations for a Python package distribution file. Contains one or more attestation bundles verified by PyPI, along with the Trusted Publisher identity that produced them.\",\n  \"type\": \"object\",\n  \"required\": [\"version\", \"attestation_bundles\"],\n  \"properties\": {\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The provenance object format version. Currently always 1.\",\n      \"enum\": [1]\n    },\n    \"attestation_bundles\": {\n      \"type\": \"array\",\n      \"description\": \"One or more attestation bundles, each containing the publisher identity and a set of attestations.\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/AttestationBundle\"\n      }\n    }\n  },\n\
  \  \"$defs\": {\n    \"AttestationBundle\": {\n      \"type\": \"object\",\n      \"description\": \"A bundle of attestations produced by a single Trusted Publisher identity.\",\n      \"required\": [\"publisher\", \"attestations\"],\n      \"properties\": {\n        \"publisher\": {\n          \"$ref\": \"#/$defs/Publisher\"\n        },\n        \"attestations\": {\n          \"type\": \"array\",\n          \"description\": \"The attestation objects in this bundle.\",\n          \"minItems\": 1,\n          \"items\": {\n            \"$ref\": \"#/$defs/Attestation\"\n          }\n        }\n      }\n    },\n    \"Publisher\": {\n      \"type\": \"object\",\n      \"description\": \"The Trusted Publisher identity that produced the attestations, verified through OpenID Connect.\",\n      \"required\": [\"kind\"],\n      \"properties\": {\n        \"kind\": {\n          \"type\": \"string\",\n          \"description\": \"The type of Trusted Publisher, indicating the CI/CD platform.\",\n \
  \         \"enum\": [\"GitHub\", \"GitLab\", \"Google\", \"ActiveState\"]\n        },\n        \"claims\": {\n          \"type\": \"object\",\n          \"description\": \"Identity claims from the OIDC token, such as repository and workflow information.\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"vendor-property\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"An optional vendor-specific property providing additional publisher context.\"\n        }\n      }\n    },\n    \"Attestation\": {\n      \"type\": \"object\",\n      \"description\": \"A single attestation for a distribution file, containing the attestation type and a Sigstore bundle.\",\n      \"required\": [\"version\", \"verification_material\", \"envelope\"],\n      \"properties\": {\n        \"version\": {\n          \"type\": \"integer\",\n          \"description\": \"The attestation object version. Currently always 1.\",\n \
  \         \"enum\": [1]\n        },\n        \"verification_material\": {\n          \"type\": \"object\",\n          \"description\": \"Sigstore verification material including the signing certificate and transparency log entries.\",\n          \"properties\": {\n            \"certificate\": {\n              \"type\": \"string\",\n              \"description\": \"The base64-encoded signing certificate from the Sigstore CA.\"\n            },\n            \"transparency_entries\": {\n              \"type\": \"array\",\n              \"description\": \"Entries from the Sigstore transparency log (Rekor).\",\n              \"items\": {\n                \"type\": \"object\",\n                \"description\": \"A single transparency log entry.\",\n                \"additionalProperties\": true\n              }\n            }\n          }\n        },\n        \"envelope\": {\n          \"type\": \"object\",\n          \"description\": \"The DSSE envelope containing the signed attestation statement.\"\
  ,\n          \"properties\": {\n            \"statement\": {\n              \"type\": \"string\",\n              \"description\": \"The base64-encoded attestation statement.\"\n            },\n            \"signature\": {\n              \"type\": \"string\",\n              \"description\": \"The base64-encoded signature over the statement.\"\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/pypi/refs/heads/main/json-schema/pypi-provenance-schema.json
tags:
- Developer Tools
- Open Source
- Package Management
- Packages
- Python
title: PyPI Provenance
---
