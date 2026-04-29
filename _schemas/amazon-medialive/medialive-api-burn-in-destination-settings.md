---
description: Burn In Destination Settings
layout: schema
name: BurnInDestinationSettings
properties_list:
- description: ''
  name: Alignment
  type: object
- description: ''
  name: BackgroundColor
  type: object
- description: ''
  name: BackgroundOpacity
  type: object
- description: ''
  name: Font
  type: object
- description: ''
  name: FontColor
  type: object
- description: ''
  name: FontOpacity
  type: object
- description: ''
  name: FontResolution
  type: object
- description: ''
  name: FontSize
  type: object
- description: ''
  name: OutlineColor
  type: object
- description: ''
  name: OutlineSize
  type: object
- description: ''
  name: ShadowColor
  type: object
- description: ''
  name: ShadowOpacity
  type: object
- description: ''
  name: ShadowXOffset
  type: object
- description: ''
  name: ShadowYOffset
  type: object
- description: ''
  name: TeletextGridControl
  type: object
- description: ''
  name: XPosition
  type: object
- description: ''
  name: YPosition
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-burn-in-destination-settings-schema.json
slug: medialive-api-burn-in-destination-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-burn-in-destination-settings-schema.json\",\n  \"title\": \"BurnInDestinationSettings\",\n  \"description\": \"Burn In Destination Settings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInAlignment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"alignment\"\n          },\n          \"description\": \"If no explicit xPosition or yPosition is provided, setting alignment to centered will place the captions at the bottom center of the output. Similarly, setting a left alignment will align captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative\
  \ to those coordinates. Selecting \\\"smart\\\" justification will left-justify live subtitles and center-justify pre-recorded subtitles.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"BackgroundColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInBackgroundColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"backgroundColor\"\n          },\n          \"description\": \"Specifies the color of the rectangle behind the captions.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"BackgroundOpacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"backgroundOpacity\"\n          },\n          \"description\": \"Specifies the opacity of the background rectangle. 255 is opaque; 0 is transparent. Leaving this parameter out is equivalent\
  \ to setting it to 0 (transparent).  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"Font\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputLocation\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"font\"\n          },\n          \"description\": \"External font file used for caption burn-in. File extension must be 'ttf' or 'tte'.  Although the user can select output fonts for many different types of input captions,  embedded, STL and teletext sources use a strict grid system. Using external fonts with these caption sources could cause unexpected display of proportional fonts.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"FontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInFontColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontColor\"\n          },\n          \"description\"\
  : \"Specifies the color of the burned-in captions.  This option is not valid for source captions that are STL, 608/embedded or teletext.  These source settings are already pre-defined by the caption stream.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"FontOpacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontOpacity\"\n          },\n          \"description\": \"Specifies the opacity of the burned-in captions. 255 is opaque; 0 is transparent.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"FontResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin96Max600\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontResolution\"\n          },\n          \"description\": \"Font resolution in DPI (dots per inch); default\
  \ is 96 dpi.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"FontSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontSize\"\n          },\n          \"description\": \"When set to 'auto' fontSize will scale depending on the size of the output.  Giving a positive integer will specify the exact font size in points.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"OutlineColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInOutlineColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outlineColor\"\n          },\n          \"description\": \"Specifies font outline color. This option is not valid for source captions that are either 608/embedded or teletext. These source settings are already pre-defined by the caption stream. All burn-in\
  \ and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"OutlineSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outlineSize\"\n          },\n          \"description\": \"Specifies font outline size in pixels. This option is not valid for source captions that are either 608/embedded or teletext. These source settings are already pre-defined by the caption stream. All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"ShadowColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInShadowColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowColor\"\n          },\n          \"description\": \"Specifies the color of the shadow cast by the captions.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"ShadowOpacity\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowOpacity\"\n          },\n          \"description\": \"Specifies the opacity of the shadow. 255 is opaque; 0 is transparent. Leaving this parameter out is equivalent to setting it to 0 (transparent).  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"ShadowXOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowXOffset\"\n          },\n          \"description\": \"Specifies the horizontal offset of the shadow relative to the captions in pixels. A value of -2 would result in a shadow offset 2 pixels to the left.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"ShadowYOffset\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowYOffset\"\n          },\n          \"description\": \"Specifies the vertical offset of the shadow relative to the captions in pixels. A value of -2 would result in a shadow offset 2 pixels above the text.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"TeletextGridControl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInTeletextGridControl\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextGridControl\"\n          },\n          \"description\": \"Controls whether a fixed grid size will be used to generate the output subtitles bitmap. Only applicable for Teletext inputs and DVB-Sub/Burn-in outputs.\"\n        }\n      ]\n    },\n    \"XPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n  \
  \        \"xml\": {\n            \"name\": \"xPosition\"\n          },\n          \"description\": \"Specifies the horizontal position of the caption relative to the left side of the output in pixels. A value of 10 would result in the captions starting 10 pixels from the left of the output. If no explicit xPosition is provided, the horizontal caption position will be determined by the alignment parameter.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"YPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"yPosition\"\n          },\n          \"description\": \"Specifies the vertical position of the caption relative to the top of the output in pixels. A value of 10 would result in the captions starting 10 pixels from the top of the output. If no explicit yPosition is provided, the caption will be positioned towards the bottom of\
  \ the output.  All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-burn-in-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BurnInDestinationSettings
---
