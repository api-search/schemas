---
description: Represents an asynchronous generation task in the Runway API. Tasks are created when submitting video, image, or audio generation requests and can be polled for status and output.
layout: schema
name: Runway Generation Task
properties_list:
- description: The unique identifier for the generation task.
  name: id
  type: string
- description: The current processing status of the task.
  name: status
  type: string
- description: The ISO 8601 timestamp when the task was created.
  name: createdAt
  type: string
- description: One or more URLs linking to the generated output media. Only present when the task status is SUCCEEDED.
  name: output
  type: array
- description: A description of the failure reason. Only present when the task status is FAILED.
  name: failure
  type: string
provider_name: Runway
provider_slug: runway
schema_file: json-schema/runway-task-schema.json
slug: runway-task
source_filename: runway-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.dev.runwayml.com/schemas/runway/task.json\",\n  \"title\": \"Runway Generation Task\",\n  \"description\": \"Represents an asynchronous generation task in the Runway API. Tasks are created when submitting video, image, or audio generation requests and can be polled for status and output.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"status\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the generation task.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status of the task.\",\n      \"enum\": [\"PENDING\", \"PROCESSING\", \"SUCCEEDED\", \"FAILED\", \"CANCELLED\"]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the task\
  \ was created.\"\n    },\n    \"output\": {\n      \"type\": \"array\",\n      \"description\": \"One or more URLs linking to the generated output media. Only present when the task status is SUCCEEDED.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uri\"\n      }\n    },\n    \"failure\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the failure reason. Only present when the task status is FAILED.\"\n    }\n  },\n  \"$defs\": {\n    \"ImageToVideoInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters for image-to-video generation tasks.\",\n      \"required\": [\"model\", \"promptImage\"],\n      \"properties\": {\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The model to use for generation.\",\n          \"enum\": [\"gen4\", \"gen4_turbo\", \"gen4.5\", \"gen4_aleph\"]\n        },\n        \"promptImage\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"An HTTPS URL, runway:// URI, or data URI containing an encoded image to use as input.\"\n        },\n        \"promptText\": {\n          \"type\": \"string\",\n          \"description\": \"A text description of up to 1000 characters describing what should appear in the output.\",\n          \"maxLength\": 1000\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"description\": \"The duration of the generated video in seconds.\",\n          \"enum\": [5, 10]\n        },\n        \"ratio\": {\n          \"type\": \"string\",\n          \"description\": \"The aspect ratio of the output video.\",\n          \"enum\": [\"1280:720\", \"1584:672\", \"1104:832\", \"720:1280\", \"832:1104\", \"960:960\"]\n        }\n      }\n    },\n    \"TextToVideoInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters for text-to-video generation tasks.\",\n      \"required\": [\"model\", \"promptText\"],\n      \"properties\": {\n        \"model\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The model to use for text-to-video generation.\",\n          \"enum\": [\"gen4.5\", \"veo3.1\", \"veo3.1_fast\", \"veo3\"]\n        },\n        \"promptText\": {\n          \"type\": \"string\",\n          \"description\": \"A text description of up to 1000 characters describing what should appear in the output.\",\n          \"maxLength\": 1000\n        },\n        \"duration\": {\n          \"type\": \"integer\",\n          \"description\": \"The duration of the generated video in seconds.\",\n          \"enum\": [5, 10]\n        },\n        \"ratio\": {\n          \"type\": \"string\",\n          \"description\": \"The aspect ratio of the output video.\",\n          \"enum\": [\"1280:720\", \"1584:672\", \"1104:832\", \"720:1280\", \"832:1104\", \"960:960\"]\n        }\n      }\n    },\n    \"TextToImageInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters for text-to-image generation tasks.\"\
  ,\n      \"required\": [\"model\", \"promptText\"],\n      \"properties\": {\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The model to use for image generation.\",\n          \"enum\": [\"gen4_image\"]\n        },\n        \"promptText\": {\n          \"type\": \"string\",\n          \"description\": \"A text description of up to 1000 characters describing what should appear in the output.\",\n          \"maxLength\": 1000\n        },\n        \"ratio\": {\n          \"type\": \"string\",\n          \"description\": \"The aspect ratio of the output image.\",\n          \"enum\": [\"1280:720\", \"1584:672\", \"1104:832\", \"720:1280\", \"832:1104\", \"960:960\"]\n        }\n      }\n    },\n    \"VideoToVideoInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters for video-to-video generation tasks.\",\n      \"required\": [\"model\", \"promptVideo\", \"promptText\"],\n      \"properties\": {\n        \"model\": {\n    \
  \      \"type\": \"string\",\n          \"description\": \"The model to use for video-to-video generation.\",\n          \"enum\": [\"gen4_aleph\"]\n        },\n        \"promptVideo\": {\n          \"type\": \"string\",\n          \"description\": \"An HTTPS URL or runway:// URI pointing to the input video.\"\n        },\n        \"promptText\": {\n          \"type\": \"string\",\n          \"description\": \"A text description guiding the transformation of the input video.\",\n          \"maxLength\": 1000\n        },\n        \"ratio\": {\n          \"type\": \"string\",\n          \"description\": \"The aspect ratio of the output video.\",\n          \"enum\": [\"1280:720\", \"1584:672\", \"1104:832\", \"720:1280\", \"832:1104\", \"960:960\"]\n        }\n      }\n    },\n    \"CharacterPerformanceInput\": {\n      \"type\": \"object\",\n      \"description\": \"Input parameters for character performance (Act Two) generation tasks.\",\n      \"required\": [\"model\", \"character\",\
  \ \"reference\"],\n      \"properties\": {\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The model to use. Must be act_two.\",\n          \"enum\": [\"act_two\"]\n        },\n        \"character\": {\n          \"$ref\": \"#/$defs/MediaReference\",\n          \"description\": \"The character to animate.\"\n        },\n        \"reference\": {\n          \"$ref\": \"#/$defs/MediaReference\",\n          \"description\": \"The driving performance reference controlling the character's movements.\"\n        },\n        \"ratio\": {\n          \"type\": \"string\",\n          \"description\": \"The aspect ratio of the output video.\",\n          \"enum\": [\"1280:720\", \"1584:672\", \"1104:832\", \"720:1280\", \"832:1104\", \"960:960\"]\n        }\n      }\n    },\n    \"MediaReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a media asset (image or video) used as input.\",\n      \"required\": [\"type\", \"uri\"],\n \
  \     \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The media type of the input.\",\n          \"enum\": [\"image\", \"video\"]\n        },\n        \"uri\": {\n          \"type\": \"string\",\n          \"description\": \"An HTTPS URL or runway:// URI pointing to the media asset.\"\n        }\n      }\n    },\n    \"AspectRatio\": {\n      \"type\": \"string\",\n      \"description\": \"Supported aspect ratios for generated media. Includes landscape (1280:720, 1584:672, 1104:832), portrait (720:1280, 832:1104), and square (960:960) formats.\",\n      \"enum\": [\"1280:720\", \"1584:672\", \"1104:832\", \"720:1280\", \"832:1104\", \"960:960\"]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/json-schema/runway-task-schema.json
tags:
- Video Generation
- Image Generation
- Artificial Intelligence
- Machine Learning
- Generative AI
- Avatars
- Characters
- WebRTC
- Creative Tools
title: Runway Generation Task
---
