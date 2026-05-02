---
description: Schema for an Azure DevOps pipeline run as returned by the Pipelines REST API. A pipeline run represents a single execution of a YAML pipeline, triggered manually or by a CI/CD event. The run tracks state (inProgress, completed), result (succeeded, failed, canceled), timing, and the resources and parameters used.
layout: schema
name: Azure DevOps Pipeline Run
properties_list:
- description: Unique numeric identifier for this pipeline run. Assigned sequentially within the project.
  name: id
  type: integer
- description: Auto-generated run name, typically the build number format defined in the pipeline YAML (e.g., $(Date:yyyyMMdd).$(Rev:r)). Can be overridden by the pipeline's name property.
  name: name
  type: string
- description: Current execution state of the pipeline run.
  name: state
  type: string
- description: Final result of a completed run. Null when the run is not yet completed (state is inProgress or canceling).
  name: result
  type:
  - string
  - 'null'
- description: ISO 8601 UTC timestamp when the run was created (queued).
  name: createdDate
  type: string
- description: ISO 8601 UTC timestamp when the run finished. Null if the run has not yet completed.
  name: finishedDate
  type:
  - string
  - 'null'
- description: REST API URL for accessing this run directly.
  name: url
  type: string
- description: Reference to the pipeline definition this run belongs to.
  name: pipeline
  type: object
- description: Resources consumed by this pipeline run, such as repository checkout versions and upstream pipeline dependencies.
  name: resources
  type: object
- description: Variables used in this run. Includes both pipeline-defined variables and any overrides specified when triggering the run. Secret variable values are not returned.
  name: variables
  type:
  - object
  - 'null'
- description: Template parameters passed to the YAML pipeline for this run. Parameters are defined with `parameters:` in the pipeline YAML and allow type-safe overrides at queue time.
  name: templateParameters
  type:
  - object
  - 'null'
- description: HAL links for related resources (web view, pipeline definition, artifacts).
  name: _links
  type: object
provider_name: Azure DevOps
provider_slug: microsoft-azure-devops
schema_file: json-schema/azure-devops-pipeline-run-schema.json
slug: azure-devops-pipeline-run
source_filename: azure-devops-pipeline-run-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://learn.microsoft.com/en-us/rest/api/azure/devops/pipelines/runs/get\",\n  \"title\": \"Azure DevOps Pipeline Run\",\n  \"description\": \"Schema for an Azure DevOps pipeline run as returned by the Pipelines REST API. A pipeline run represents a single execution of a YAML pipeline, triggered manually or by a CI/CD event. The run tracks state (inProgress, completed), result (succeeded, failed, canceled), timing, and the resources and parameters used.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\", \"state\", \"pipeline\", \"url\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier for this pipeline run. Assigned sequentially within the project.\",\n      \"minimum\": 1,\n      \"examples\": [1001, 2345]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated run name,\
  \ typically the build number format defined in the pipeline YAML (e.g., $(Date:yyyyMMdd).$(Rev:r)). Can be overridden by the pipeline's name property.\",\n      \"examples\": [\"20240315.1\", \"main-20240315-1001\"]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current execution state of the pipeline run.\",\n      \"enum\": [\"unknown\", \"inProgress\", \"canceling\", \"completed\"],\n      \"examples\": [\"completed\", \"inProgress\"]\n    },\n    \"result\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Final result of a completed run. Null when the run is not yet completed (state is inProgress or canceling).\",\n      \"enum\": [\"unknown\", \"succeeded\", \"failed\", \"canceled\", null],\n      \"examples\": [\"succeeded\", \"failed\"]\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the run was created (queued).\",\n      \"\
  examples\": [\"2024-03-15T10:00:00Z\"]\n    },\n    \"finishedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 UTC timestamp when the run finished. Null if the run has not yet completed.\",\n      \"examples\": [\"2024-03-15T10:15:00Z\", null]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"REST API URL for accessing this run directly.\",\n      \"examples\": [\"https://dev.azure.com/myorg/myproject/_apis/pipelines/15/runs/1001\"]\n    },\n    \"pipeline\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to the pipeline definition this run belongs to.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"Pipeline definition ID.\",\n          \"examples\": [15]\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Pipeline definition name.\",\n          \"examples\": [\"CI Pipeline\", \"Deploy to Production\"]\n        },\n        \"folder\": {\n          \"type\": \"string\",\n          \"description\": \"Folder path where the pipeline definition is organized.\",\n          \"examples\": [\"\\\\CI\", \"\\\\Production\"]\n        },\n        \"revision\": {\n          \"type\": \"integer\",\n          \"description\": \"Revision number of the pipeline definition used for this run.\",\n          \"minimum\": 1\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"REST API URL for the pipeline definition.\",\n          \"examples\": [\"https://dev.azure.com/myorg/myproject/_apis/pipelines/15\"]\n        },\n        \"_links\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"self\": {\n              \"$ref\": \"#/$defs/HalLink\"\n            },\n            \"web\": {\n              \"$ref\"\
  : \"#/$defs/HalLink\"\n            }\n          }\n        }\n      }\n    },\n    \"resources\": {\n      \"type\": \"object\",\n      \"description\": \"Resources consumed by this pipeline run, such as repository checkout versions and upstream pipeline dependencies.\",\n      \"properties\": {\n        \"repositories\": {\n          \"type\": \"object\",\n          \"description\": \"Repository resources used in this run, keyed by repository alias (e.g., 'self' for the pipeline's own repo).\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/RepositoryResource\"\n          }\n        },\n        \"pipelines\": {\n          \"type\": \"object\",\n          \"description\": \"Pipeline resources from upstream pipelines used as inputs, keyed by pipeline alias.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/PipelineResource\"\n          }\n        },\n        \"builds\": {\n          \"type\": \"object\",\n          \"description\": \"Build\
  \ resources used in this run, keyed by resource alias.\",\n          \"additionalProperties\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"version\": {\n                \"type\": \"string\",\n                \"description\": \"Build number\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"variables\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Variables used in this run. Includes both pipeline-defined variables and any overrides specified when triggering the run. Secret variable values are not returned.\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/Variable\"\n      }\n    },\n    \"templateParameters\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Template parameters passed to the YAML pipeline for this run. Parameters are defined with `parameters:` in the pipeline YAML and allow type-safe overrides at queue time.\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\",\n        \"description\": \"Parameter value (serialized as string)\"\n      },\n      \"examples\": [\n        {\n          \"environment\": \"production\",\n          \"deployRegion\": \"eastus\",\n          \"runTests\": \"true\"\n        }\n      ]\n    },\n    \"_links\": {\n      \"type\": \"object\",\n      \"description\": \"HAL links for related resources (web view, pipeline definition, artifacts).\",\n      \"properties\": {\n        \"self\": {\n          \"$ref\": \"#/$defs/HalLink\"\n        },\n        \"web\": {\n          \"$ref\": \"#/$defs/HalLink\"\n        },\n        \"pipeline\": {\n          \"$ref\": \"#/$defs/HalLink\"\n        },\n        \"pipeline.web\": {\n          \"$ref\": \"#/$defs/HalLink\"\n        }\n      },\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/HalLink\"\n      }\n    }\n  },\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"RepositoryResource\": {\n      \"type\": \"object\",\n \
  \     \"description\": \"A repository resource used in a pipeline run\",\n      \"properties\": {\n        \"refName\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The Git ref (branch or tag) checked out for this run.\",\n          \"examples\": [\"refs/heads/main\", \"refs/heads/feature/login\", \"refs/tags/v1.2.3\"]\n        },\n        \"version\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The specific commit SHA checked out for this run.\",\n          \"examples\": [\"a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4e5f6a1b2\"]\n        },\n        \"repository\": {\n          \"type\": \"object\",\n          \"description\": \"Repository details\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\",\n              \"description\": \"Repository GUID\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n              \"description\": \"Repository name\"\n            },\n\
  \            \"type\": {\n              \"type\": \"string\",\n              \"description\": \"Repository type\",\n              \"enum\": [\"unknown\", \"azureReposGit\", \"gitHub\", \"azureReposGitHyphenated\"]\n            },\n            \"url\": {\n              \"type\": \"string\",\n              \"format\": \"uri\"\n            }\n          }\n        }\n      }\n    },\n    \"PipelineResource\": {\n      \"type\": \"object\",\n      \"description\": \"A pipeline resource from an upstream pipeline run\",\n      \"properties\": {\n        \"pipeline\": {\n          \"type\": \"object\",\n          \"description\": \"Reference to the upstream pipeline\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"integer\"\n            },\n            \"name\": {\n              \"type\": \"string\"\n            },\n            \"folder\": {\n              \"type\": \"string\"\n            },\n            \"url\": {\n              \"type\": \"string\",\n      \
  \        \"format\": \"uri\"\n            }\n          }\n        },\n        \"version\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Build number of the upstream pipeline run used\"\n        }\n      }\n    },\n    \"Variable\": {\n      \"type\": \"object\",\n      \"description\": \"A pipeline variable value\",\n      \"properties\": {\n        \"value\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The variable value. Null for secret variables (values are redacted in API responses).\"\n        },\n        \"isSecret\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether this variable is marked as secret. Secret variables are not returned in API responses.\",\n          \"default\": false\n        }\n      }\n    },\n    \"HalLink\": {\n      \"type\": \"object\",\n      \"description\": \"A HAL hypertext link\",\n      \"required\": [\"href\"],\n      \"properties\": {\n        \"href\": {\n   \
  \       \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL target of the link\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-devops/refs/heads/main/json-schema/azure-devops-pipeline-run-schema.json
tags:
- Agile
- CI/CD
- DevOps
- Project Management
- Version Control
title: Azure DevOps Pipeline Run
---
