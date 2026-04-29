---
description: Burn-in is a captions delivery method, rather than a captions format. Burn-in writes the captions directly on your video frames, replacing pixels of video content with the captions. Set up burn-in captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/burn-in-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to BURN_IN.
layout: schema
name: BurninDestinationSettings
properties_list:
- description: ''
  name: Alignment
  type: object
- description: ''
  name: ApplyFontColor
  type: object
- description: ''
  name: BackgroundColor
  type: object
- description: ''
  name: BackgroundOpacity
  type: object
- description: ''
  name: FallbackFont
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
  name: FontScript
  type: object
- description: ''
  name: FontSize
  type: object
- description: ''
  name: HexFontColor
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
  name: StylePassthrough
  type: object
- description: ''
  name: TeletextSpacing
  type: object
- description: ''
  name: XPosition
  type: object
- description: ''
  name: YPosition
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-burnin-destination-settings-schema.json
slug: mediaconvert-api-burnin-destination-settings
source_filename: mediaconvert-api-burnin-destination-settings-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-burnin-destination-settings-schema.json\",\n  \"title\": \"BurninDestinationSettings\",\n  \"description\": \"Burn-in is a captions delivery method, rather than a captions format. Burn-in writes the captions directly on your video frames, replacing pixels of video content with the captions. Set up burn-in captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/burn-in-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to BURN_IN.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleAlignment\"\n        },\n       \
  \ {\n          \"xml\": {\n            \"name\": \"alignment\"\n          },\n          \"description\": \"Specify the alignment of your captions. If no explicit x_position is provided, setting alignment to centered will placethe captions at the bottom center of the output. Similarly, setting a left alignment willalign captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative to those coordinates.\"\n        }\n      ]\n    },\n    \"ApplyFontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleApplyFontColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"applyFontColor\"\n          },\n          \"description\": \"Ignore this setting unless Style passthrough (StylePassthrough) is set to Enabled and Font color (FontColor) set to Black, Yellow, Red, Green, Blue, or Hex. Use Apply font color (ApplyFontColor)\
  \ for additional font color controls. When you choose White text only (WHITE_TEXT_ONLY), or leave blank, your font color setting only applies to white text in your input captions. For example, if your font color setting is Yellow, and your input captions have red and white text, your output captions will have red and yellow text. When you choose ALL_TEXT, your font color setting applies to all of your output captions text.\"\n        }\n      ]\n    },\n    \"BackgroundColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleBackgroundColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"backgroundColor\"\n          },\n          \"description\": \"Specify the color of the rectangle behind the captions. Leave background color (BackgroundColor) blank and set Style passthrough (StylePassthrough) to enabled to use the background color data from your input captions, if present.\"\n        }\n      ]\n    },\n    \"BackgroundOpacity\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"backgroundOpacity\"\n          },\n          \"description\": \"Specify the opacity of the background rectangle. Enter a value from 0 to 255, where 0 is transparent and 255 is opaque. If Style passthrough (StylePassthrough) is set to enabled, leave blank to pass through the background style information in your input captions to your output captions. If Style passthrough is set to disabled, leave blank to use a value of 0 and remove all backgrounds from your output captions.\"\n        }\n      ]\n    },\n    \"FallbackFont\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleFallbackFont\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fallbackFont\"\n          },\n          \"description\": \"Specify the font that you want the service to use for your burn\
  \ in captions when your input captions specify a font that MediaConvert doesn't support. When you set Fallback font (FallbackFont) to best match (BEST_MATCH), or leave blank, MediaConvert uses a supported font that most closely matches the font that your input captions specify. When there are multiple unsupported fonts in your input captions, MediaConvert matches each font with the supported font that matches best. When you explicitly choose a replacement font, MediaConvert uses that font to replace all unsupported fonts from your input.\"\n        }\n      ]\n    },\n    \"FontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleFontColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontColor\"\n          },\n          \"description\": \"Specify the color of the burned-in captions text. Leave Font color (FontColor) blank and set Style passthrough (StylePassthrough) to enabled to use the font color data from your\
  \ input captions, if present.\"\n        }\n      ]\n    },\n    \"FontOpacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontOpacity\"\n          },\n          \"description\": \"Specify the opacity of the burned-in captions. 255 is opaque; 0 is transparent.\"\n        }\n      ]\n    },\n    \"FontResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin96Max600\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontResolution\"\n          },\n          \"description\": \"Specify the Font resolution (FontResolution) in DPI (dots per inch).\"\n        }\n      ]\n    },\n    \"FontScript\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FontScript\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontScript\"\n          },\n          \"description\"\
  : \"Set Font script (FontScript) to Automatically determined (AUTOMATIC), or leave blank, to automatically determine the font script in your input captions. Otherwise, set to Simplified Chinese (HANS) or Traditional Chinese (HANT) if your input font script uses Simplified or Traditional Chinese.\"\n        }\n      ]\n    },\n    \"FontSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max96\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontSize\"\n          },\n          \"description\": \"Specify the Font size (FontSize) in pixels. Must be a positive integer. Set to 0, or leave blank, for automatic font size.\"\n        }\n      ]\n    },\n    \"HexFontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin6Max8Pattern09aFAF609aFAF2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hexFontColor\"\n          },\n          \"description\": \"Ignore this\
  \ setting unless your Font color is set to Hex. Enter either six or eight hexidecimal digits, representing red, green, and blue, with two optional extra digits for alpha. For example a value of 1122AABB is a red value of 0x11, a green value of 0x22, a blue value of 0xAA, and an alpha value of 0xBB.\"\n        }\n      ]\n    },\n    \"OutlineColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleOutlineColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outlineColor\"\n          },\n          \"description\": \"Specify font outline color. Leave Outline color (OutlineColor) blank and set Style passthrough (StylePassthrough) to enabled to use the font outline color data from your input captions, if present.\"\n        }\n      ]\n    },\n    \"OutlineSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"outlineSize\"\n          },\n          \"description\": \"Specify the Outline size (OutlineSize) of the caption text, in pixels. Leave Outline size blank and set Style passthrough (StylePassthrough) to enabled to use the outline size data from your input captions, if present.\"\n        }\n      ]\n    },\n    \"ShadowColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleShadowColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowColor\"\n          },\n          \"description\": \"Specify the color of the shadow cast by the captions. Leave Shadow color (ShadowColor) blank and set Style passthrough (StylePassthrough) to enabled to use the shadow color data from your input captions, if present.\"\n        }\n      ]\n    },\n    \"ShadowOpacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"shadowOpacity\"\n          },\n          \"description\": \"Specify the opacity of the shadow. Enter a value from 0 to 255, where 0 is transparent and 255 is opaque. If Style passthrough (StylePassthrough) is set to Enabled, leave Shadow opacity (ShadowOpacity) blank to pass through the shadow style information in your input captions to your output captions. If Style passthrough is set to disabled, leave blank to use a value of 0 and remove all shadows from your output captions.\"\n        }\n      ]\n    },\n    \"ShadowXOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowXOffset\"\n          },\n          \"description\": \"Specify the horizontal offset of the shadow, relative to the captions in pixels. A value of -2 would result in a shadow offset 2 pixels to the left.\"\n        }\n      ]\n    },\n    \"ShadowYOffset\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowYOffset\"\n          },\n          \"description\": \"Specify the vertical offset of the shadow relative to the captions in pixels. A value of -2 would result in a shadow offset 2 pixels above the text. Leave Shadow y-offset (ShadowYOffset) blank and set Style passthrough (StylePassthrough) to enabled to use the shadow y-offset data from your input captions, if present.\"\n        }\n      ]\n    },\n    \"StylePassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurnInSubtitleStylePassthrough\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"stylePassthrough\"\n          },\n          \"description\": \"Set Style passthrough (StylePassthrough) to ENABLED to use the available style, color, and position information from your input captions.\
  \ MediaConvert uses default settings for any missing style and position information in your input captions. Set Style passthrough to DISABLED, or leave blank, to ignore the style and position information from your input captions and use default settings: white text with black outlining, bottom-center positioning, and automatic sizing. Whether you set Style passthrough to enabled or not, you can also choose to manually override any of the individual style and position settings.\"\n        }\n      ]\n    },\n    \"TeletextSpacing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BurninSubtitleTeletextSpacing\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextSpacing\"\n          },\n          \"description\": \"Specify whether the text spacing (TeletextSpacing) in your captions is set by the captions grid, or varies depending on letter width. Choose fixed grid (FIXED_GRID) to conform to the spacing specified in the captions file\
  \ more accurately. Choose proportional (PROPORTIONAL) to make the text easier to read for closed captions.\"\n        }\n      ]\n    },\n    \"XPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xPosition\"\n          },\n          \"description\": \"Specify the horizontal position (XPosition) of the captions, relative to the left side of the output in pixels. A value of 10 would result in the captions starting 10 pixels from the left of the output. If no explicit x_position is provided, the horizontal caption position will be determined by the alignment parameter.\"\n        }\n      ]\n    },\n    \"YPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"yPosition\"\n          },\n          \"description\": \"Specify\
  \ the vertical position (YPosition) of the captions, relative to the top of the output in pixels. A value of 10 would result in the captions starting 10 pixels from the top of the output. If no explicit y_position is provided, the caption will be positioned towards the bottom of the output.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-burnin-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BurninDestinationSettings
---
