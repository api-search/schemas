---
description: Summary information about a pipeline execution.
layout: schema
name: PipelineExecutionSummary
properties_list:
- description: ''
  name: pipelineExecutionId
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: lastUpdateTime
  type: object
- description: ''
  name: sourceRevisions
  type: object
- description: ''
  name: trigger
  type: object
- description: ''
  name: stopTrigger
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-execution-summary-schema.json
slug: amazon-codepipeline-pipeline-execution-summary
source_filename: amazon-codepipeline-pipeline-execution-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-execution-summary-schema.json\",\n  \"title\": \"PipelineExecutionSummary\",\n  \"description\": \"Summary information about a pipeline execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the pipeline execution.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionStatus\"\n        },\n        {\n          \"description\": \"<p>The status of the pipeline execution.</p> <ul> <li> <p>InProgress: The pipeline execution is currently running.</p> </li> <li> <p>Stopped: The pipeline execution\
  \ was manually stopped. For more information, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/concepts.html#concepts-executions-stopped\\\">Stopped Executions</a>.</p> </li> <li> <p>Stopping: The pipeline execution received a request to be manually stopped. Depending on the selected stop mode, the execution is either completing or abandoning in-progress actions. For more information, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/concepts.html#concepts-executions-stopped\\\">Stopped Executions</a>.</p> </li> <li> <p>Succeeded: The pipeline execution was completed successfully. </p> </li> <li> <p>Superseded: While this pipeline execution was waiting for the next stage to be completed, a newer pipeline execution advanced and continued through the pipeline instead. For more information, see <a href=\\\"https://docs.aws.amazon.com/codepipeline/latest/userguide/concepts.html#concepts-superseded\\\">Superseded Executions</a>.</p> </li> <li>\
  \ <p>Failed: The pipeline execution was not completed successfully.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time when the pipeline execution began, in timestamp format.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time of the last change to the pipeline execution, in timestamp format.\"\n        }\n      ]\n    },\n    \"sourceRevisions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceRevisionList\"\n        },\n        {\n          \"description\": \"A list of the source artifact revisions that initiated a pipeline execution.\"\n        }\n      ]\n    },\n    \"trigger\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/ExecutionTrigger\"\n        },\n        {\n          \"description\": \"The interaction or event that started a pipeline execution, such as automated change detection or a <code>StartPipelineExecution</code> API call.\"\n        }\n      ]\n    },\n    \"stopTrigger\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopExecutionTrigger\"\n        },\n        {\n          \"description\": \"The interaction that stopped a pipeline execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-execution-summary-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineExecutionSummary
---
