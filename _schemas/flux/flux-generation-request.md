---
description: JSON Schema for image generation requests submitted to the Black Forest Labs Flux API. Covers the common parameters shared across FLUX model variants and the asynchronous task response format.
layout: schema
name: Flux Image Generation Request
properties_list:
- description: Text description of the image to generate. Detailed prompts with subject, style, lighting, and composition details yield the best results.
  name: prompt
  type: string
- description: Width of the output image in pixels. Must be a multiple of 32. Used with height for standard generation endpoints.
  name: width
  type: integer
- description: Height of the output image in pixels. Must be a multiple of 32.
  name: height
  type: integer
- description: Aspect ratio for Ultra model generation. Used instead of explicit width/height.
  name: aspect_ratio
  type: string
- description: Number of diffusion inference steps. More steps increase quality but also processing time.
  name: steps
  type: integer
- description: Classifier-free guidance scale. Higher values adhere more closely to the prompt; lower values allow more creative variation.
  name: guidance
  type: number
- description: Random seed for reproducible generation. Omit for a random seed.
  name: seed
  type: integer
- description: Content safety filter level from 0 (most restrictive) to 6 (least restrictive). Default is 2.
  name: safety_tolerance
  type: integer
- description: Output image file format.
  name: output_format
  type: string
- description: Whether to automatically enhance the prompt using an LLM before generation.
  name: prompt_upsampling
  type: boolean
- description: Ultra model only. If true, produces more natural photorealistic images without additional artistic processing.
  name: raw
  type: boolean
provider_name: Flux
provider_slug: flux
schema_file: json-schema/flux-generation-request-schema.json
slug: flux-generation-request
source_filename: flux-generation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/flux/blob/main/json-schema/flux-generation-request-schema.json\",\n  \"title\": \"Flux Image Generation Request\",\n  \"description\": \"JSON Schema for image generation requests submitted to the Black Forest Labs Flux API. Covers the common parameters shared across FLUX model variants and the asynchronous task response format.\",\n  \"type\": \"object\",\n  \"required\": [\"prompt\"],\n  \"properties\": {\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"Text description of the image to generate. Detailed prompts with subject, style, lighting, and composition details yield the best results.\",\n      \"maxLength\": 10000\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"description\": \"Width of the output image in pixels. Must be a multiple of 32. Used with height for standard generation endpoints.\",\n      \"minimum\"\
  : 256,\n      \"maximum\": 1440\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"description\": \"Height of the output image in pixels. Must be a multiple of 32.\",\n      \"minimum\": 256,\n      \"maximum\": 1440\n    },\n    \"aspect_ratio\": {\n      \"type\": \"string\",\n      \"description\": \"Aspect ratio for Ultra model generation. Used instead of explicit width/height.\",\n      \"enum\": [\"21:9\", \"16:9\", \"4:3\", \"3:2\", \"1:1\", \"2:3\", \"3:4\", \"9:16\", \"9:21\"]\n    },\n    \"steps\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of diffusion inference steps. More steps increase quality but also processing time.\",\n      \"minimum\": 1,\n      \"maximum\": 50\n    },\n    \"guidance\": {\n      \"type\": \"number\",\n      \"description\": \"Classifier-free guidance scale. Higher values adhere more closely to the prompt; lower values allow more creative variation.\",\n      \"minimum\": 1.5,\n      \"maximum\": 10.0\n    },\n\
  \    \"seed\": {\n      \"type\": \"integer\",\n      \"description\": \"Random seed for reproducible generation. Omit for a random seed.\",\n      \"minimum\": 0\n    },\n    \"safety_tolerance\": {\n      \"type\": \"integer\",\n      \"description\": \"Content safety filter level from 0 (most restrictive) to 6 (least restrictive). Default is 2.\",\n      \"minimum\": 0,\n      \"maximum\": 6,\n      \"default\": 2\n    },\n    \"output_format\": {\n      \"type\": \"string\",\n      \"description\": \"Output image file format.\",\n      \"enum\": [\"jpeg\", \"png\"],\n      \"default\": \"jpeg\"\n    },\n    \"prompt_upsampling\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to automatically enhance the prompt using an LLM before generation.\",\n      \"default\": false\n    },\n    \"raw\": {\n      \"type\": \"boolean\",\n      \"description\": \"Ultra model only. If true, produces more natural photorealistic images without additional artistic processing.\",\n\
  \      \"default\": false\n    }\n  },\n  \"$defs\": {\n    \"TaskResponse\": {\n      \"type\": \"object\",\n      \"title\": \"TaskResponse\",\n      \"description\": \"Response returned immediately when a generation or editing request is submitted. The caller must poll the get_result endpoint with the returned ID.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Unique task identifier. Use this to poll GET /v1/get_result?id={id}.\"\n        },\n        \"polling_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Pre-built polling URL for convenience.\"\n        }\n      }\n    },\n    \"ResultResponse\": {\n      \"type\": \"object\",\n      \"title\": \"ResultResponse\",\n      \"description\": \"Response from polling the generation result. When status is Ready, the result contains a download URL.\",\n    \
  \  \"required\": [\"id\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"Task identifier matching the original request.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Current task status. Poll until Ready or an error state.\",\n          \"enum\": [\"Pending\", \"Processing\", \"Ready\", \"Error\", \"Content Moderated\", \"Request Moderated\"]\n        },\n        \"result\": {\n          \"$ref\": \"#/$defs/GenerationResult\"\n        }\n      }\n    },\n    \"GenerationResult\": {\n      \"type\": \"object\",\n      \"title\": \"GenerationResult\",\n      \"description\": \"The successful output of a completed image generation or editing task.\",\n      \"properties\": {\n        \"sample\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"Pre-signed URL to download the generated\
  \ or edited image. This URL expires after a short time.\"\n        },\n        \"prompt\": {\n          \"type\": \"string\",\n          \"description\": \"The effective prompt used for generation, which may differ from the submitted prompt if prompt_upsampling was enabled.\"\n        },\n        \"seed\": {\n          \"type\": \"integer\",\n          \"description\": \"The random seed that was used for this generation. Useful for reproducing the same result.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"KontextEditRequest\": {\n      \"type\": \"object\",\n      \"title\": \"KontextEditRequest\",\n      \"description\": \"Request body for FLUX.1 Kontext image editing. Extends the base generation request with an input image field.\",\n      \"required\": [\"prompt\", \"image\"],\n      \"properties\": {\n        \"prompt\": {\n          \"type\": \"string\",\n          \"description\": \"Text instruction describing the desired edit to apply to the input image.\",\n \
  \         \"maxLength\": 10000\n        },\n        \"image\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded input image to edit. Supported formats are JPEG and PNG.\",\n          \"contentEncoding\": \"base64\",\n          \"contentMediaType\": \"image/jpeg\"\n        },\n        \"steps\": {\n          \"type\": \"integer\",\n          \"description\": \"Diffusion inference steps.\",\n          \"minimum\": 1,\n          \"maximum\": 50\n        },\n        \"guidance\": {\n          \"type\": \"number\",\n          \"description\": \"Guidance scale.\",\n          \"minimum\": 1.5,\n          \"maximum\": 10.0\n        },\n        \"seed\": {\n          \"type\": \"integer\",\n          \"description\": \"Random seed.\",\n          \"minimum\": 0\n        },\n        \"safety_tolerance\": {\n          \"type\": \"integer\",\n          \"description\": \"Safety filter level (0-6).\",\n          \"minimum\": 0,\n          \"maximum\": 6\n        },\n \
  \       \"output_format\": {\n          \"type\": \"string\",\n          \"description\": \"Output format.\",\n          \"enum\": [\"jpeg\", \"png\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/flux/refs/heads/main/json-schema/flux-generation-request-schema.json
tags:
- AI
- Image Generation
- Machine Learning
- Open Source
- Text to Image
title: Flux Image Generation Request
---
