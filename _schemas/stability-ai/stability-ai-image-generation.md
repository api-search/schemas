---
description: Schema representing the configuration and response structures for Stability AI image generation operations including text-to-image, image-to-image, editing, upscaling, and control-guided generation.
layout: schema
name: Stability AI Image Generation
properties_list:
- description: ''
  name: prompt
  type: object
- description: Text describing elements to exclude from the output image.
  name: negative_prompt
  type: string
- description: ''
  name: aspect_ratio
  type: object
- description: ''
  name: output_format
  type: object
- description: ''
  name: seed
  type: object
- description: ''
  name: model
  type: object
- description: ''
  name: mode
  type: object
- description: Controls how much influence the input image has on the output for image-to-image mode.
  name: strength
  type: number
- description: Controls how closely the output follows the input control image.
  name: control_strength
  type: number
provider_name: stability-ai
provider_slug: stability-ai
schema_file: json-schema/stability-ai-image-generation-schema.json
slug: stability-ai-image-generation
source_filename: stability-ai-image-generation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://stability.ai/schemas/stability-ai/image-generation.json\",\n  \"title\": \"Stability AI Image Generation\",\n  \"description\": \"Schema representing the configuration and response structures for Stability AI image generation operations including text-to-image, image-to-image, editing, upscaling, and control-guided generation.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"Prompt\": {\n      \"type\": \"object\",\n      \"description\": \"Text prompt configuration for guiding image generation.\",\n      \"required\": [\"text\"],\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\",\n          \"maxLength\": 10000,\n          \"description\": \"Text describing what should appear in the generated image. Strong, descriptive prompts that clearly define elements, colors, and subjects lead to better results.\"\n        },\n        \"weight\": {\n          \"type\"\
  : \"number\",\n          \"description\": \"The weight of the prompt relative to other prompts. Higher values give this prompt more influence.\"\n        }\n      }\n    },\n    \"AspectRatio\": {\n      \"type\": \"string\",\n      \"description\": \"The aspect ratio of the generated image.\",\n      \"enum\": [\n        \"16:9\",\n        \"1:1\",\n        \"21:9\",\n        \"2:3\",\n        \"3:2\",\n        \"4:5\",\n        \"5:4\",\n        \"9:16\",\n        \"9:21\"\n      ]\n    },\n    \"OutputFormat\": {\n      \"type\": \"string\",\n      \"description\": \"The output format of the generated image.\",\n      \"enum\": [\"jpeg\", \"png\", \"webp\"]\n    },\n    \"Seed\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 4294967294,\n      \"description\": \"A value to control randomness in generation. Set to 0 for a random seed. Using the same seed with the same parameters produces similar results.\"\n    },\n    \"GenerationModel\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The model variant used for generation.\",\n      \"enum\": [\n        \"sd3\",\n        \"sd3-turbo\",\n        \"sd3.5-large\",\n        \"sd3.5-large-turbo\",\n        \"sd3.5-medium\",\n        \"stable-image-core\",\n        \"stable-image-ultra\"\n      ]\n    },\n    \"GenerationMode\": {\n      \"type\": \"string\",\n      \"description\": \"The generation mode indicating whether this is a text-to-image or image-to-image operation.\",\n      \"enum\": [\"text-to-image\", \"image-to-image\"]\n    },\n    \"FinishReason\": {\n      \"type\": \"string\",\n      \"description\": \"The reason the generation finished.\",\n      \"enum\": [\"SUCCESS\", \"CONTENT_FILTERED\"]\n    },\n    \"GenerationResult\": {\n      \"type\": \"object\",\n      \"description\": \"The result of an image generation operation.\",\n      \"properties\": {\n        \"image\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded image data.\"\
  \n        },\n        \"finish_reason\": {\n          \"$ref\": \"#/$defs/FinishReason\"\n        },\n        \"seed\": {\n          \"$ref\": \"#/$defs/Seed\"\n        }\n      }\n    },\n    \"AsyncGeneration\": {\n      \"type\": \"object\",\n      \"description\": \"Response for an asynchronous generation that must be polled for results.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The unique generation ID used to poll for results.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The current status of the generation.\"\n        }\n      }\n    },\n    \"EditOperation\": {\n      \"type\": \"string\",\n      \"description\": \"The type of image editing operation.\",\n      \"enum\": [\n        \"inpaint\",\n        \"outpaint\",\n        \"erase\",\n        \"search-and-replace\",\n        \"search-and-recolor\",\n        \"remove-background\"\
  ,\n        \"replace-background-and-relight\"\n      ]\n    },\n    \"ControlMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The method of structural control for image-to-image generation.\",\n      \"enum\": [\"sketch\", \"structure\", \"style\"]\n    },\n    \"UpscaleMethod\": {\n      \"type\": \"string\",\n      \"description\": \"The upscaling method to use.\",\n      \"enum\": [\"fast\", \"conservative\", \"creative\"]\n    },\n    \"OutpaintExtension\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for outpainting extension directions.\",\n      \"properties\": {\n        \"left\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of pixels to extend to the left.\"\n        },\n        \"right\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of pixels to extend to the right.\"\n        },\n        \"up\": {\n          \"type\": \"integer\"\
  ,\n          \"minimum\": 0,\n          \"description\": \"Number of pixels to extend upward.\"\n        },\n        \"down\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Number of pixels to extend downward.\"\n        }\n      }\n    },\n    \"ImageToVideoConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for image-to-video generation.\",\n      \"properties\": {\n        \"seed\": {\n          \"$ref\": \"#/$defs/Seed\"\n        },\n        \"cfg_scale\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 10,\n          \"description\": \"Controls how closely the video follows the conditioning from the input image.\"\n        },\n        \"motion_bucket_id\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"maximum\": 255,\n          \"description\": \"Controls the amount of motion in the generated video.\"\n        }\n      }\n    },\n    \"Fast3DConfig\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Configuration for Stable Fast 3D mesh generation.\",\n      \"properties\": {\n        \"texture_resolution\": {\n          \"type\": \"integer\",\n          \"enum\": [512, 1024, 2048],\n          \"description\": \"The resolution of the generated texture in pixels.\"\n        },\n        \"foreground_ratio\": {\n          \"type\": \"number\",\n          \"minimum\": 0.1,\n          \"maximum\": 1.0,\n          \"description\": \"The ratio of the foreground object to the total image size.\"\n        },\n        \"remesh\": {\n          \"type\": \"string\",\n          \"enum\": [\"none\", \"triangle\", \"quad\"],\n          \"description\": \"The remeshing algorithm to apply to the generated mesh.\"\n        }\n      }\n    },\n    \"ApiError\": {\n      \"type\": \"object\",\n      \"description\": \"An error response from the Stability AI API.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n\
  \          \"description\": \"A unique identifier for the error instance.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The error type name.\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the error.\"\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"prompt\": {\n      \"$ref\": \"#/$defs/Prompt\"\n    },\n    \"negative_prompt\": {\n      \"type\": \"string\",\n      \"maxLength\": 10000,\n      \"description\": \"Text describing elements to exclude from the output image.\"\n    },\n    \"aspect_ratio\": {\n      \"$ref\": \"#/$defs/AspectRatio\"\n    },\n    \"output_format\": {\n      \"$ref\": \"#/$defs/OutputFormat\"\n    },\n    \"seed\": {\n      \"$ref\": \"#/$defs/Seed\"\n    },\n    \"model\": {\n      \"$ref\": \"#/$defs/GenerationModel\"\n    },\n    \"mode\": {\n      \"$ref\": \"#/$defs/GenerationMode\"\n    },\n    \"strength\"\
  : {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Controls how much influence the input image has on the output for image-to-image mode.\"\n    },\n    \"control_strength\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 1,\n      \"description\": \"Controls how closely the output follows the input control image.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/stability-ai/refs/heads/main/json-schema/stability-ai-image-generation-schema.json
tags: []
title: Stability AI Image Generation
---
