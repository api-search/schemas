---
description: Represents an asynchronous image generation job in the Midjourney API, including its configuration parameters, current status, and generation results.
layout: schema
name: Midjourney Image Generation Job
properties_list:
- description: The unique identifier assigned to this image generation job.
  name: id
  type: string
- description: The type of image generation operation performed by this job.
  name: type
  type: string
- description: The current processing status of the job.
  name: status
  type: string
- description: The completion progress as a percentage from 0 to 100.
  name: progress
  type: integer
- description: The text prompt submitted for image generation.
  name: prompt
  type: string
- description: ''
  name: parameters
  type: object
- description: The job identifier of the parent generation, present for upscale and variation jobs.
  name: parent_job_id
  type: string
- description: The index of the selected image from the parent job grid, present for upscale and variation jobs.
  name: image_index
  type: integer
- description: ''
  name: result
  type: object
- description: ''
  name: error
  type: object
- description: The webhook URL configured to receive status change notifications for this job.
  name: webhook_url
  type: string
- description: Controls when webhook notifications are delivered for this job.
  name: webhook_type
  type: string
- description: ISO 8601 timestamp when the job was created.
  name: created_at
  type: string
- description: ISO 8601 timestamp when the job was last updated.
  name: updated_at
  type: string
- description: ISO 8601 timestamp when the job completed processing.
  name: completed_at
  type: string
provider_name: midjourney
provider_slug: midjourney
schema_file: json-schema/midjourney-image-generation-job-schema.json
slug: midjourney-image-generation-job
source_filename: midjourney-image-generation-job-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://midjourney.com/schemas/image-generation-job.json\",\n  \"title\": \"Midjourney Image Generation Job\",\n  \"description\": \"Represents an asynchronous image generation job in the Midjourney API, including its configuration parameters, current status, and generation results.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"status\", \"created_at\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier assigned to this image generation job.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of image generation operation performed by this job.\",\n      \"enum\": [\"imagine\", \"upscale\", \"variation\", \"describe\", \"blend\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status of the\
  \ job.\",\n      \"enum\": [\"pending\", \"in_progress\", \"completed\", \"failed\", \"cancelled\"]\n    },\n    \"progress\": {\n      \"type\": \"integer\",\n      \"description\": \"The completion progress as a percentage from 0 to 100.\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"The text prompt submitted for image generation.\",\n      \"maxLength\": 4000\n    },\n    \"parameters\": {\n      \"$ref\": \"#/$defs/GenerationParameters\"\n    },\n    \"parent_job_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The job identifier of the parent generation, present for upscale and variation jobs.\"\n    },\n    \"image_index\": {\n      \"type\": \"integer\",\n      \"description\": \"The index of the selected image from the parent job grid, present for upscale and variation jobs.\",\n      \"minimum\": 1,\n      \"maximum\": 4\n    },\n    \"result\": {\n \
  \     \"$ref\": \"#/$defs/JobResult\"\n    },\n    \"error\": {\n      \"$ref\": \"#/$defs/JobError\"\n    },\n    \"webhook_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The webhook URL configured to receive status change notifications for this job.\"\n    },\n    \"webhook_type\": {\n      \"type\": \"string\",\n      \"description\": \"Controls when webhook notifications are delivered for this job.\",\n      \"enum\": [\"progress\", \"result\"],\n      \"default\": \"result\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the job was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the job was last updated.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601\
  \ timestamp when the job completed processing.\"\n    }\n  },\n  \"$defs\": {\n    \"GenerationParameters\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration parameters that control the image generation process.\",\n      \"properties\": {\n        \"aspect_ratio\": {\n          \"type\": \"string\",\n          \"description\": \"The aspect ratio for generated images, expressed as width:height.\",\n          \"pattern\": \"^[0-9]+:[0-9]+$\",\n          \"default\": \"1:1\"\n        },\n        \"model_version\": {\n          \"type\": \"string\",\n          \"description\": \"The Midjourney model version used for generation.\",\n          \"enum\": [\"5.2\", \"6.0\", \"6.1\", \"7.0\"]\n        },\n        \"process_mode\": {\n          \"type\": \"string\",\n          \"description\": \"The processing speed mode for the generation job.\",\n          \"enum\": [\"fast\", \"turbo\", \"relax\"],\n          \"default\": \"fast\"\n        },\n        \"quality\": {\n \
  \         \"type\": \"number\",\n          \"description\": \"The quality setting controlling detail level and GPU time consumption.\",\n          \"enum\": [0.25, 0.5, 1.0, 2.0],\n          \"default\": 1.0\n        },\n        \"stylize\": {\n          \"type\": \"integer\",\n          \"description\": \"The stylization strength from 0 (literal) to 1000 (highly artistic).\",\n          \"minimum\": 0,\n          \"maximum\": 1000,\n          \"default\": 100\n        },\n        \"chaos\": {\n          \"type\": \"integer\",\n          \"description\": \"Controls the diversity between the four generated images in a grid.\",\n          \"minimum\": 0,\n          \"maximum\": 100,\n          \"default\": 0\n        },\n        \"seed\": {\n          \"type\": \"integer\",\n          \"description\": \"Seed value for reproducible generation results.\",\n          \"minimum\": 0,\n          \"maximum\": 4294967295\n        },\n        \"no\": {\n          \"type\": \"string\",\n        \
  \  \"description\": \"Negative prompt specifying elements to exclude from generated images.\"\n        }\n      }\n    },\n    \"JobResult\": {\n      \"type\": \"object\",\n      \"description\": \"The output of a successfully completed image generation job.\",\n      \"properties\": {\n        \"images\": {\n          \"type\": \"array\",\n          \"description\": \"List of generated images with download URLs and metadata.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/GeneratedImage\"\n          }\n        },\n        \"prompts\": {\n          \"type\": \"array\",\n          \"description\": \"Generated text prompt suggestions, present only for describe job results.\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"GeneratedImage\": {\n      \"type\": \"object\",\n      \"description\": \"A single generated image with its metadata and download URL.\",\n      \"required\": [\"url\"],\n      \"properties\": {\n\
  \        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL where the generated image can be downloaded.\"\n        },\n        \"index\": {\n          \"type\": \"integer\",\n          \"description\": \"The position of this image in the generation grid (1-4).\",\n          \"minimum\": 1,\n          \"maximum\": 4\n        },\n        \"width\": {\n          \"type\": \"integer\",\n          \"description\": \"The width of the image in pixels.\",\n          \"minimum\": 1\n        },\n        \"height\": {\n          \"type\": \"integer\",\n          \"description\": \"The height of the image in pixels.\",\n          \"minimum\": 1\n        },\n        \"content_type\": {\n          \"type\": \"string\",\n          \"description\": \"The MIME type of the image file.\",\n          \"enum\": [\"image/png\", \"image/webp\"]\n        }\n      }\n    },\n    \"JobError\": {\n      \"type\": \"object\",\n      \"description\":\
  \ \"Error information for a failed image generation job.\",\n      \"required\": [\"code\", \"message\"],\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Machine-readable error code identifying the type of failure.\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable description of the error.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/midjourney/refs/heads/main/json-schema/midjourney-image-generation-job-schema.json
tags: []
title: Midjourney Image Generation Job
---
