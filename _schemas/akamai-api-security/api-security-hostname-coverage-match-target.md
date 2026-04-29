---
description: Contains details about a hostname coverage match target.
layout: schema
name: hostname-coverage-match-target
properties_list:
- description: The list of API endpoint identifiers and names. This applies only for `api` match targets.
  name: apis
  type: array
- description: The network lists' identifiers and names in the match target.
  name: bypassNetworkLists
  type: array
- description: Describes the rule to match on paths. Either `NO_MATCH` not to match on the default file, `BASE_MATCH` to match only requests for top-level hostnames ending in a trailing slash, or `RECURSIVE_MATCH` t
  name: defaultFile
  type: string
- description: __Read-only__ The security controls to apply. For a security control to be effectively turned on, you must enable it in both the match target and the security policy.
  name: effectiveSecurityControls
  type: object
- description: The list of file extensions to apply the match target to.
  name: fileExtensions
  type: array
- description: The list of file paths to apply the match target to.
  name: filePaths
  type: array
- description: The list of hostnames to protect.
  name: hostnames
  type: array
- description: Whether the match target applies when a match is found in the specified `fileExtensions` or when a match isn't found.
  name: isNegativeFileExtensionMatch
  type: boolean
- description: Whether the match target applies when a match is found in the specified `filePaths` or when a match isn't found.
  name: isNegativePathMatch
  type: boolean
- description: The security policy associated with the match target.
  name: securityPolicy
  type: object
- description: The match target's position in the sequence of match targets.
  name: sequence
  type: integer
- description: Uniquely identifies the match target.
  name: targetId
  type: integer
- description: The type of match target. Either `website` or `api`.
  name: type
  type: string
- description: __Read-only__ Contains details about warnings, errors, or notices determined by a validation of this resource.
  name: validations
  type: object
provider_name: Akamai API Security
provider_slug: akamai-api-security
schema_file: json-schema/api-security-hostname-coverage-match-target-schema.json
slug: api-security-hostname-coverage-match-target
source_filename: api-security-hostname-coverage-match-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostname-coverage-match-target-schema.json\",\n  \"title\": \"hostname-coverage-match-target\",\n  \"description\": \"Contains details about a hostname coverage match target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apis\": {\n      \"description\": \"The list of API endpoint identifiers and names. This applies only for `api` match targets.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Uniquely identifies the API endpoint.\",\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"description\": \"The API endpoint name.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ],\n      \
  \  \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"bypassNetworkLists\": {\n      \"description\": \"The network lists' identifiers and names in the match target.\",\n      \"items\": {\n        \"additionalProperties\": false,\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Uniquely identifies the network list.\",\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"description\": \"The name you assigned to the network list.\",\n            \"type\": \"string\"\n          }\n        },\n        \"required\": [\n          \"id\"\n        ],\n        \"type\": \"object\"\n      },\n      \"type\": \"array\"\n    },\n    \"defaultFile\": {\n      \"default\": \"NO_MATCH\",\n      \"description\": \"Describes the rule to match on paths. Either `NO_MATCH` not to match on the default file, `BASE_MATCH` to match only requests for top-level hostnames ending in a trailing slash, or `RECURSIVE_MATCH` to match\
  \ all requests for paths that end in a trailing slash. The default value is `NO_MATCH`.\",\n      \"enum\": [\n        \"NO_MATCH\",\n        \"BASE_MATCH\",\n        \"RECURSIVE_MATCH\"\n      ],\n      \"type\": \"string\"\n    },\n    \"effectiveSecurityControls\": {\n      \"additionalProperties\": false,\n      \"description\": \"__Read-only__ The security controls to apply. For a security control to be effectively turned on, you must enable it in both the match target and the security policy.\",\n      \"properties\": {\n        \"applyApiConstraints\": {\n          \"description\": \"Whether you enabled API constraints.\",\n          \"type\": \"boolean\"\n        },\n        \"applyApplicationLayerControls\": {\n          \"description\": \"Whether you enabled application layer controls.\",\n          \"type\": \"boolean\"\n        },\n        \"applyBotmanControls\": {\n          \"description\": \"Whether you enabled Bot Manager controls.\",\n          \"type\": \"boolean\"\n\
  \        },\n        \"applyNetworkLayerControls\": {\n          \"description\": \"Whether you enabled network layer controls.\",\n          \"type\": \"boolean\"\n        },\n        \"applyRateControls\": {\n          \"description\": \"Whether you enabled rate controls.\",\n          \"type\": \"boolean\"\n        },\n        \"applyReputationControls\": {\n          \"description\": \"Whether you enabled reputation controls.\",\n          \"type\": \"boolean\"\n        },\n        \"applySlowPostControls\": {\n          \"description\": \"Whether you enabled slow post controls.\",\n          \"type\": \"boolean\"\n        }\n      },\n      \"readOnly\": true,\n      \"required\": [\n        \"applyApplicationLayerControls\",\n        \"applyNetworkLayerControls\",\n        \"applyRateControls\",\n        \"applyReputationControls\",\n        \"applyBotmanControls\",\n        \"applyApiConstraints\",\n        \"applySlowPostControls\"\n      ],\n      \"type\": \"object\",\n     \
  \ \"x-akamai\": {\n        \"file-path\": \"schemas/security-controls.yaml\"\n      }\n    },\n    \"fileExtensions\": {\n      \"description\": \"The list of file extensions to apply the match target to.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"filePaths\": {\n      \"description\": \"The list of file paths to apply the match target to.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"hostnames\": {\n      \"description\": \"The list of hostnames to protect.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    },\n    \"isNegativeFileExtensionMatch\": {\n      \"description\": \"Whether the match target applies when a match is found in the specified `fileExtensions` or when a match isn't found.\",\n      \"type\": \"boolean\"\n    },\n    \"isNegativePathMatch\": {\n      \"description\": \"Whether the match target applies when\
  \ a match is found in the specified `filePaths` or when a match isn't found.\",\n      \"type\": \"boolean\"\n    },\n    \"securityPolicy\": {\n      \"additionalProperties\": false,\n      \"description\": \"The security policy associated with the match target.\",\n      \"properties\": {\n        \"policyId\": {\n          \"description\": \"Uniquely identifies the security policy.\",\n          \"type\": \"string\"\n        }\n      },\n      \"required\": [\n        \"policyId\"\n      ],\n      \"type\": \"object\"\n    },\n    \"sequence\": {\n      \"description\": \"The match target's position in the sequence of match targets.\",\n      \"type\": \"integer\"\n    },\n    \"targetId\": {\n      \"description\": \"Uniquely identifies the match target.\",\n      \"type\": \"integer\"\n    },\n    \"type\": {\n      \"description\": \"The type of match target. Either `website` or `api`.\",\n      \"enum\": [\n        \"website\",\n        \"api\"\n      ],\n      \"type\": \"string\"\
  \n    },\n    \"validations\": {\n      \"additionalProperties\": false,\n      \"description\": \"__Read-only__ Contains details about warnings, errors, or notices determined by a validation of this resource.\",\n      \"properties\": {\n        \"errors\": {\n          \"description\": \"The list of errors.\",\n          \"items\": {\n            \"additionalProperties\": false,\n            \"description\": \"Contains feedback on validation.\",\n            \"properties\": {\n              \"detail\": {\n                \"description\": \"The explanation of the error message.\",\n                \"type\": \"string\"\n              },\n              \"fieldName\": {\n                \"description\": \"The name of the field causing the validation problem.\",\n                \"type\": \"string\"\n              },\n              \"jsonReference\": {\n                \"description\": \"The JSON reference to the field in the resource.\",\n                \"type\": \"string\"\n          \
  \    },\n              \"title\": {\n                \"description\": \"The title for the error.\",\n                \"example\": \"Not Found\",\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"description\": \"The URL for the error type.\",\n                \"example\": \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"title\",\n              \"type\"\n            ],\n            \"type\": \"object\",\n            \"x-akamai\": {\n              \"file-path\": \"schemas/validation.yaml\"\n            }\n          },\n          \"type\": \"array\"\n        },\n        \"notices\": {\n          \"description\": \"The list of notices.\",\n          \"items\": {\n            \"additionalProperties\": false,\n            \"description\": \"Contains feedback on validation.\",\n            \"properties\": {\n              \"detail\"\
  : {\n                \"description\": \"The explanation of the error message.\",\n                \"type\": \"string\"\n              },\n              \"fieldName\": {\n                \"description\": \"The name of the field causing the validation problem.\",\n                \"type\": \"string\"\n              },\n              \"jsonReference\": {\n                \"description\": \"The JSON reference to the field in the resource.\",\n                \"type\": \"string\"\n              },\n              \"title\": {\n                \"description\": \"The title for the error.\",\n                \"example\": \"Not Found\",\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"description\": \"The URL for the error type.\",\n                \"example\": \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"title\",\n           \
  \   \"type\"\n            ],\n            \"type\": \"object\",\n            \"x-akamai\": {\n              \"file-path\": \"schemas/validation.yaml\"\n            }\n          },\n          \"type\": \"array\"\n        },\n        \"warnings\": {\n          \"description\": \"The list of warnings.\",\n          \"items\": {\n            \"additionalProperties\": false,\n            \"description\": \"Contains feedback on validation.\",\n            \"properties\": {\n              \"detail\": {\n                \"description\": \"The explanation of the error message.\",\n                \"type\": \"string\"\n              },\n              \"fieldName\": {\n                \"description\": \"The name of the field causing the validation problem.\",\n                \"type\": \"string\"\n              },\n              \"jsonReference\": {\n                \"description\": \"The JSON reference to the field in the resource.\",\n                \"type\": \"string\"\n              },\n   \
  \           \"title\": {\n                \"description\": \"The title for the error.\",\n                \"example\": \"Not Found\",\n                \"type\": \"string\"\n              },\n              \"type\": {\n                \"description\": \"The URL for the error type.\",\n                \"example\": \"/appsec/problem-types/INCOMPATIBLE-FIELD\",\n                \"type\": \"string\"\n              }\n            },\n            \"required\": [\n              \"title\",\n              \"type\"\n            ],\n            \"type\": \"object\",\n            \"x-akamai\": {\n              \"file-path\": \"schemas/validation.yaml\"\n            }\n          },\n          \"type\": \"array\"\n        }\n      },\n      \"readOnly\": true,\n      \"required\": [\n        \"notices\",\n        \"errors\",\n        \"warnings\"\n      ],\n      \"type\": \"object\",\n      \"x-akamai\": {\n        \"file-path\": \"schemas/validations.yaml\"\n      }\n    }\n  },\n  \"required\": [\n\
  \    \"type\",\n    \"securityPolicy\"\n  ],\n  \"additionalProperties\": false\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/json-schema/api-security-hostname-coverage-match-target-schema.json
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
title: hostname-coverage-match-target
---
