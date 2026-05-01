---
description: Schema for a Binary Authorization policy, which defines the rules for deploying container images to Google Cloud environments.
layout: schema
name: Google Cloud Binary Authorization Policy
properties_list:
- description: The resource name of the policy
  name: name
  type: string
- description: Whether to enable the global policy evaluation mode
  name: globalPolicyEvaluationMode
  type: string
- description: Image name patterns that are always allowed to be deployed
  name: admissionWhitelistPatterns
  type: array
- description: The default admission rule for the policy
  name: defaultAdmissionRule
  type: object
- description: Per-cluster admission rules keyed by cluster resource ID
  name: clusterAdmissionRules
  type: object
- description: Per-namespace admission rules
  name: kubernetesNamespaceAdmissionRules
  type: object
- description: Per-service-account admission rules
  name: kubernetesServiceAccountAdmissionRules
  type: object
- description: The time when the policy was last updated
  name: updateTime
  type: string
provider_name: Google Cloud Binary Authorization
provider_slug: google-cloud-binary-authorization
schema_file: json-schema/google-cloud-binary-authorization-policy-schema.json
slug: google-cloud-binary-authorization-policy
source_filename: google-cloud-binary-authorization-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/binaryauthorization/policy.json\",\n  \"title\": \"Google Cloud Binary Authorization Policy\",\n  \"description\": \"Schema for a Binary Authorization policy, which defines the rules for deploying container images to Google Cloud environments.\",\n  \"type\": \"object\",\n  \"required\": [\"defaultAdmissionRule\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the policy\"\n    },\n    \"globalPolicyEvaluationMode\": {\n      \"type\": \"string\",\n      \"description\": \"Whether to enable the global policy evaluation mode\",\n      \"enum\": [\"ENABLE\", \"DISABLE\"]\n    },\n    \"admissionWhitelistPatterns\": {\n      \"type\": \"array\",\n      \"description\": \"Image name patterns that are always allowed to be deployed\",\n      \"items\": {\n        \"$ref\": \"#/$defs/AdmissionWhitelistPattern\"\
  \n      }\n    },\n    \"defaultAdmissionRule\": {\n      \"$ref\": \"#/$defs/AdmissionRule\",\n      \"description\": \"The default admission rule for the policy\"\n    },\n    \"clusterAdmissionRules\": {\n      \"type\": \"object\",\n      \"description\": \"Per-cluster admission rules keyed by cluster resource ID\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/AdmissionRule\"\n      }\n    },\n    \"kubernetesNamespaceAdmissionRules\": {\n      \"type\": \"object\",\n      \"description\": \"Per-namespace admission rules\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/AdmissionRule\"\n      }\n    },\n    \"kubernetesServiceAccountAdmissionRules\": {\n      \"type\": \"object\",\n      \"description\": \"Per-service-account admission rules\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/AdmissionRule\"\n      }\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"The time when the policy was last updated\"\n    }\n  },\n  \"$defs\": {\n    \"AdmissionRule\": {\n      \"type\": \"object\",\n      \"description\": \"An admission rule specifies what action to take when a container image matches the rule\",\n      \"required\": [\"evaluationMode\", \"enforcementMode\"],\n      \"properties\": {\n        \"evaluationMode\": {\n          \"type\": \"string\",\n          \"description\": \"How this admission rule will be evaluated\",\n          \"enum\": [\"ALWAYS_ALLOW\", \"ALWAYS_DENY\", \"REQUIRE_ATTESTATION\"]\n        },\n        \"requireAttestationsBy\": {\n          \"type\": \"array\",\n          \"description\": \"Resource names of attestors required by this rule\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"enforcementMode\": {\n          \"type\": \"string\",\n          \"description\": \"The action when a pod creation is denied by the admission rule\",\n          \"enum\": [\"ENFORCED_BLOCK_AND_AUDIT_LOG\"\
  , \"DRYRUN_AUDIT_LOG_ONLY\"]\n        }\n      }\n    },\n    \"AdmissionWhitelistPattern\": {\n      \"type\": \"object\",\n      \"description\": \"An image name pattern to allow\",\n      \"properties\": {\n        \"namePattern\": {\n          \"type\": \"string\",\n          \"description\": \"An image name pattern to allowlist, in the form registry/path/to/image\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-binary-authorization/refs/heads/main/json-schema/google-cloud-binary-authorization-policy-schema.json
tags:
- Attestation
- Container Security
- DevSecOps
- Kubernetes
- Policy Enforcement
- Supply Chain Security
title: Google Cloud Binary Authorization Policy
---
