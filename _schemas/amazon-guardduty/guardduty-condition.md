---
description: Contains information about the condition.
layout: schema
name: Condition
properties_list:
- description: ''
  name: Eq
  type: object
- description: ''
  name: Neq
  type: object
- description: ''
  name: Gt
  type: object
- description: ''
  name: Gte
  type: object
- description: ''
  name: Lt
  type: object
- description: ''
  name: Lte
  type: object
- description: ''
  name: Equals
  type: object
- description: ''
  name: NotEquals
  type: object
- description: ''
  name: GreaterThan
  type: object
- description: ''
  name: GreaterThanOrEqual
  type: object
- description: ''
  name: LessThan
  type: object
- description: ''
  name: LessThanOrEqual
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-condition-schema.json
slug: guardduty-condition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-condition-schema.json\",\n  \"title\": \"Condition\",\n  \"description\": \"Contains information about the condition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Eq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Eq\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"eq\"\n          },\n          \"description\": \"Represents the <i>equal</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"Neq\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Neq\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"neq\"\n          },\n          \"description\": \"Represents\
  \ the <i>not equal</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"Gt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"gt\"\n          },\n          \"description\": \"Represents a <i>greater than</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"Gte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"gte\"\n          },\n          \"description\": \"Represents a <i>greater than or equal</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"Lt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\
  \n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"lt\"\n          },\n          \"description\": \"Represents a <i>less than</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"Lte\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"deprecated\": true,\n          \"xml\": {\n            \"name\": \"lte\"\n          },\n          \"description\": \"Represents a <i>less than or equal</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"Equals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Equals\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"equals\"\n          },\n          \"description\": \"Represents an <i>equal</i> <b/> condition to be applied to a single field when querying for findings.\"\
  \n        }\n      ]\n    },\n    \"NotEquals\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotEquals\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"notEquals\"\n          },\n          \"description\": \"Represents a <i>not equal</i> <b/> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"GreaterThan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"greaterThan\"\n          },\n          \"description\": \"Represents a <i>greater than</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"GreaterThanOrEqual\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"greaterThanOrEqual\"\n          },\n          \"description\"\
  : \"Represents a <i>greater than or equal</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"LessThan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lessThan\"\n          },\n          \"description\": \"Represents a <i>less than</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    },\n    \"LessThanOrEqual\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"lessThanOrEqual\"\n          },\n          \"description\": \"Represents a <i>less than or equal</i> condition to be applied to a single field when querying for findings.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-condition-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Condition
---
