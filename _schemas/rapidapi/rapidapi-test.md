---
description: Schema representing an API test configuration in RapidAPI Testing, including test steps, assertions, schedules, and execution results.
layout: schema
name: RapidAPI Test
properties_list:
- description: Unique identifier for the test
  name: id
  type: string
- description: Display name of the test
  name: name
  type: string
- description: Description of what the test validates
  name: description
  type: string
- description: The API this test is associated with on the RapidAPI Hub
  name: apiId
  type: string
- description: The type of test to execute
  name: type
  type: string
- description: Current status of the test configuration
  name: status
  type: string
- description: Ordered list of test steps that execute sequentially
  name: steps
  type: array
- description: Optional schedule for automated test execution
  name: schedule
  type: object
- description: Environment variables used during test execution
  name: environment
  type: object
- description: Result of the most recent test execution
  name: lastExecution
  type: object
- description: Timestamp when the test was created
  name: createdAt
  type: string
- description: Timestamp when the test was last modified
  name: updatedAt
  type: string
provider_name: RapidAPI
provider_slug: rapidapi
schema_file: json-schema/rapidapi-test-schema.json
slug: rapidapi-test
source_filename: rapidapi-test-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://rapidapi.com/schemas/rapidapi/test.json\",\n  \"title\": \"RapidAPI Test\",\n  \"description\": \"Schema representing an API test configuration in RapidAPI Testing, including test steps, assertions, schedules, and execution results.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"steps\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the test\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the test\",\n      \"minLength\": 1,\n      \"maxLength\": 200\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the test validates\"\n    },\n    \"apiId\": {\n      \"type\": \"string\",\n      \"description\": \"The API this test is associated with on the RapidAPI Hub\"\n    },\n    \"type\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\"functional\", \"performance\"],\n      \"description\": \"The type of test to execute\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"draft\", \"archived\"],\n      \"description\": \"Current status of the test configuration\"\n    },\n    \"steps\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TestStep\"\n      },\n      \"minItems\": 1,\n      \"description\": \"Ordered list of test steps that execute sequentially\"\n    },\n    \"schedule\": {\n      \"$ref\": \"#/$defs/Schedule\",\n      \"description\": \"Optional schedule for automated test execution\"\n    },\n    \"environment\": {\n      \"$ref\": \"#/$defs/Environment\",\n      \"description\": \"Environment variables used during test execution\"\n    },\n    \"lastExecution\": {\n      \"$ref\": \"#/$defs/ExecutionResult\",\n      \"description\": \"Result of the most recent test execution\"\n    },\n    \"createdAt\": {\n     \
  \ \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the test was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the test was last modified\"\n    }\n  },\n  \"$defs\": {\n    \"TestStep\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"method\", \"url\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the step\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Step name for identification in results\"\n        },\n        \"method\": {\n          \"type\": \"string\",\n          \"enum\": [\"GET\", \"POST\", \"PUT\", \"PATCH\", \"DELETE\"],\n          \"description\": \"HTTP method for the API call\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n  \
  \        \"description\": \"The endpoint URL to call, may include environment variable references\"\n        },\n        \"headers\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"HTTP headers to include in the request\"\n        },\n        \"body\": {\n          \"type\": \"string\",\n          \"description\": \"Request body content, supports variable interpolation from previous steps\"\n        },\n        \"assertions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Assertion\"\n          },\n          \"description\": \"Assertions to validate the response\"\n        },\n        \"variableExtractions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/VariableExtraction\"\n          },\n          \"description\": \"Variables to extract from the response for use in subsequent steps\"\n      \
  \  }\n      },\n      \"description\": \"A single step in a test flow that makes an API call and validates the response\"\n    },\n    \"Assertion\": {\n      \"type\": \"object\",\n      \"required\": [\"target\", \"comparison\"],\n      \"properties\": {\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"The response element to assert on, such as status_code, response_time, or a JSONPath expression\"\n        },\n        \"comparison\": {\n          \"type\": \"string\",\n          \"enum\": [\"equals\", \"not_equals\", \"contains\", \"not_contains\", \"greater_than\", \"less_than\", \"exists\", \"not_exists\"],\n          \"description\": \"The comparison operator to apply\"\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The expected value to compare against\"\n        }\n      },\n      \"description\": \"An assertion that validates a specific aspect of an API response\"\n    },\n    \"VariableExtraction\"\
  : {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"source\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Variable name to store the extracted value as\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"JSONPath or header expression to extract the value from\"\n        }\n      },\n      \"description\": \"Extraction rule for chaining data between test steps\"\n    },\n    \"Schedule\": {\n      \"type\": \"object\",\n      \"required\": [\"frequency\", \"locationIds\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the schedule\"\n        },\n        \"frequency\": {\n          \"type\": \"string\",\n          \"enum\": [\"5m\", \"15m\", \"30m\", \"1h\", \"6h\", \"12h\", \"24h\"],\n          \"description\": \"How often the test should run\"\n        },\n        \"locationIds\"\
  : {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"minItems\": 1,\n          \"description\": \"AWS regions or custom locations to run the test from\"\n        },\n        \"environmentId\": {\n          \"type\": \"string\",\n          \"description\": \"The environment to use for scheduled runs\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the schedule is currently active\"\n        }\n      },\n      \"description\": \"Configuration for automated periodic test execution\"\n    },\n    \"Environment\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the environment\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Environment name such as development, staging, or\
  \ production\"\n        },\n        \"variables\": {\n          \"type\": \"object\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Key-value pairs of environment variables\"\n        }\n      },\n      \"description\": \"A set of variables representing a deployment environment\"\n    },\n    \"ExecutionResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the execution\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"passed\", \"failed\", \"running\", \"error\"],\n          \"description\": \"Overall execution result status\"\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Total execution time in milliseconds\"\n        },\n        \"location\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"The monitoring location where the test ran\"\n        },\n        \"stepResults\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/StepResult\"\n          },\n          \"description\": \"Per-step execution results\"\n        },\n        \"startedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the execution started\"\n        },\n        \"completedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp when the execution completed\"\n        }\n      },\n      \"description\": \"The result of a single test execution\"\n    },\n    \"StepResult\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"stepId\": {\n          \"type\": \"string\",\n          \"description\": \"The step that was executed\"\n        },\n        \"status\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"passed\", \"failed\", \"error\", \"skipped\"],\n          \"description\": \"Step execution result\"\n        },\n        \"responseTime\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Response time in milliseconds\"\n        },\n        \"statusCode\": {\n          \"type\": \"integer\",\n          \"description\": \"HTTP status code returned\"\n        },\n        \"assertionResults\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"passed\": {\n                \"type\": \"boolean\",\n                \"description\": \"Whether the assertion passed\"\n              },\n              \"expected\": {\n                \"type\": \"string\",\n                \"description\": \"The expected value\"\n              },\n              \"actual\": {\n                \"type\": \"string\",\n                \"description\": \"The actual\
  \ value received\"\n              }\n            }\n          },\n          \"description\": \"Results for each assertion in this step\"\n        }\n      },\n      \"description\": \"The result of executing a single test step\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rapidapi/refs/heads/main/json-schema/rapidapi-test-schema.json
tags:
- API Marketplace
- API Management
- API Testing
- API Gateway
- API Design
- Enterprise
title: RapidAPI Test
---
