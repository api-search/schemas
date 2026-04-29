---
description: Settings related to DVB-Sub captions. Set up DVB-Sub captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/dvb-sub-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to DVB_SUB.
layout: schema
name: DvbSubDestinationSettings
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
  name: DdsHandling
  type: object
- description: ''
  name: DdsXCoordinate
  type: object
- description: ''
  name: DdsYCoordinate
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
  name: Height
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
  name: SubtitlingType
  type: object
- description: ''
  name: TeletextSpacing
  type: object
- description: ''
  name: Width
  type: object
- description: ''
  name: XPosition
  type: object
- description: ''
  name: YPosition
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-dvb-sub-destination-settings-schema.json
slug: mediaconvert-api-dvb-sub-destination-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sub-destination-settings-schema.json\",\n  \"title\": \"DvbSubDestinationSettings\",\n  \"description\": \"Settings related to DVB-Sub captions. Set up DVB-Sub captions in the same output as your video. For more information, see https://docs.aws.amazon.com/mediaconvert/latest/ug/dvb-sub-output-captions.html. When you work directly in your JSON job specification, include this object and any required children when you set destinationType to DVB_SUB.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alignment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleAlignment\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"alignment\"\n          },\n          \"description\": \"Specify the alignment of your captions. If\
  \ no explicit x_position is provided, setting alignment to centered will placethe captions at the bottom center of the output. Similarly, setting a left alignment willalign captions to the bottom left of the output. If x and y positions are given in conjunction with the alignment parameter, the font will be justified (either left or centered) relative to those coordinates. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"ApplyFontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleApplyFontColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"applyFontColor\"\n          },\n          \"description\": \"Ignore this setting unless Style Passthrough (StylePassthrough) is set to Enabled and Font color (FontColor) set to Black, Yellow, Red, Green, Blue, or Hex. Use Apply font color (ApplyFontColor) for additional font color controls. When you choose White text only\
  \ (WHITE_TEXT_ONLY), or leave blank, your font color setting only applies to white text in your input captions. For example, if your font color setting is Yellow, and your input captions have red and white text, your output captions will have red and yellow text. When you choose ALL_TEXT, your font color setting applies to all of your output captions text.\"\n        }\n      ]\n    },\n    \"BackgroundColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleBackgroundColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"backgroundColor\"\n          },\n          \"description\": \"Specify the color of the rectangle behind the captions. Leave background color (BackgroundColor) blank and set Style passthrough (StylePassthrough) to enabled to use the background color data from your input captions, if present.\"\n        }\n      ]\n    },\n    \"BackgroundOpacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"backgroundOpacity\"\n          },\n          \"description\": \"Specify the opacity of the background rectangle. Enter a value from 0 to 255, where 0 is transparent and 255 is opaque. If Style passthrough (StylePassthrough) is set to enabled, leave blank to pass through the background style information in your input captions to your output captions. If Style passthrough is set to disabled, leave blank to use a value of 0 and remove all backgrounds from your output captions. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"DdsHandling\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbddsHandling\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ddsHandling\"\n          },\n          \"description\": \"Specify how MediaConvert handles the display definition segment (DDS). To exclude the DDS from this set\
  \ of captions: Keep the default, None. To include the DDS: Choose Specified. When you do, also specify the offset coordinates of the display window with DDS x-coordinate and DDS y-coordinate. To include the DDS, but not include display window data: Choose No display window. When you do, you can write position metadata to the page composition segment (PCS) with DDS x-coordinate and DDS y-coordinate. For video resolutions with a height of 576 pixels or less, MediaConvert doesn't include the DDS, regardless of the value you choose for DDS handling. All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"DdsXCoordinate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ddsXCoordinate\"\n          },\n          \"description\": \"Use this setting, along with DDS y-coordinate (ddsYCoordinate), to specify the upper left corner of the display\
  \ definition segment (DDS) display window. With this setting, specify the distance, in pixels, between the left side of the frame and the left side of the DDS display window. Keep the default value, 0, to have MediaConvert automatically choose this offset. Related setting: When you use this setting, you must set DDS handling (ddsHandling) to a value other than None (NONE). MediaConvert uses these values to determine whether to write page position data to the DDS or to the page composition segment (PCS). All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"DdsYCoordinate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ddsYCoordinate\"\n          },\n          \"description\": \"Use this setting, along with DDS x-coordinate (ddsXCoordinate), to specify the upper left corner of the display definition segment (DDS) display window.\
  \ With this setting, specify the distance, in pixels, between the top of the frame and the top of the DDS display window. Keep the default value, 0, to have MediaConvert automatically choose this offset. Related setting: When you use this setting, you must set DDS handling (ddsHandling) to a value other than None (NONE). MediaConvert uses these values to determine whether to write page position data to the DDS or to the page composition segment (PCS). All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"FallbackFont\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubSubtitleFallbackFont\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fallbackFont\"\n          },\n          \"description\": \"Specify the font that you want the service to use for your burn in captions when your input captions specify a font that MediaConvert doesn't support. When you set Fallback font (FallbackFont) to best match\
  \ (BEST_MATCH), or leave blank, MediaConvert uses a supported font that most closely matches the font that your input captions specify. When there are multiple unsupported fonts in your input captions, MediaConvert matches each font with the supported font that matches best. When you explicitly choose a replacement font, MediaConvert uses that font to replace all unsupported fonts from your input.\"\n        }\n      ]\n    },\n    \"FontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleFontColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontColor\"\n          },\n          \"description\": \"Specify the color of the captions text. Leave Font color (FontColor) blank and set Style passthrough (StylePassthrough) to enabled to use the font color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"FontOpacity\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontOpacity\"\n          },\n          \"description\": \"Specify the opacity of the burned-in captions. 255 is opaque; 0 is transparent.\\nWithin your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"FontResolution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin96Max600\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontResolution\"\n          },\n          \"description\": \"Specify the Font resolution (FontResolution) in DPI (dots per inch).\\nWithin your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"FontScript\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FontScript\"\n        },\n        {\n          \"xml\": {\n\
  \            \"name\": \"fontScript\"\n          },\n          \"description\": \"Set Font script (FontScript) to Automatically determined (AUTOMATIC), or leave blank, to automatically determine the font script in your input captions. Otherwise, set to Simplified Chinese (HANS) or Traditional Chinese (HANT) if your input font script uses Simplified or Traditional Chinese. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"FontSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max96\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"fontSize\"\n          },\n          \"description\": \"Specify the Font size (FontSize) in pixels. Must be a positive integer. Set to 0, or leave blank, for automatic font size. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"Height\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"height\"\n          },\n          \"description\": \"Specify the height, in pixels, of this set of DVB-Sub captions. The default value is 576 pixels. Related setting: When you use this setting, you must set DDS handling (ddsHandling) to a value other than None (NONE). All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"HexFontColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__stringMin6Max8Pattern09aFAF609aFAF2\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"hexFontColor\"\n          },\n          \"description\": \"Ignore this setting unless your Font color is set to Hex. Enter either six or eight hexidecimal digits, representing red, green, and blue, with two optional extra digits for alpha. For example a value of 1122AABB is a red value of 0x11, a\
  \ green value of 0x22, a blue value of 0xAA, and an alpha value of 0xBB.\"\n        }\n      ]\n    },\n    \"OutlineColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleOutlineColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outlineColor\"\n          },\n          \"description\": \"Specify font outline color. Leave Outline color (OutlineColor) blank and set Style passthrough (StylePassthrough) to enabled to use the font outline color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"OutlineSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max10\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"outlineSize\"\n          },\n          \"description\": \"Specify the Outline size (OutlineSize) of the caption text, in pixels. Leave Outline size blank\
  \ and set Style passthrough (StylePassthrough) to enabled to use the outline size data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"ShadowColor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleShadowColor\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowColor\"\n          },\n          \"description\": \"Specify the color of the shadow cast by the captions. Leave Shadow color (ShadowColor) blank and set Style passthrough (StylePassthrough) to enabled to use the shadow color data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"ShadowOpacity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max255\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowOpacity\"\
  \n          },\n          \"description\": \"Specify the opacity of the shadow. Enter a value from 0 to 255, where 0 is transparent and 255 is opaque. If Style passthrough (StylePassthrough) is set to Enabled, leave Shadow opacity (ShadowOpacity) blank to pass through the shadow style information in your input captions to your output captions. If Style passthrough is set to disabled, leave blank to use a value of 0 and remove all shadows from your output captions. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"ShadowXOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowXOffset\"\n          },\n          \"description\": \"Specify the horizontal offset of the shadow, relative to the captions in pixels. A value of -2 would result in a shadow offset 2 pixels to the left. Within\
  \ your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"ShadowYOffset\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMinNegative2147483648Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"shadowYOffset\"\n          },\n          \"description\": \"Specify the vertical offset of the shadow relative to the captions in pixels. A value of -2 would result in a shadow offset 2 pixels above the text. Leave Shadow y-offset (ShadowYOffset) blank and set Style passthrough (StylePassthrough) to enabled to use the shadow y-offset data from your input captions, if present. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"StylePassthrough\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleStylePassthrough\"\n        },\n        {\n          \"xml\": {\n            \"name\"\
  : \"stylePassthrough\"\n          },\n          \"description\": \"Set Style passthrough (StylePassthrough) to ENABLED to use the available style, color, and position information from your input captions. MediaConvert uses default settings for any missing style and position information in your input captions. Set Style passthrough to DISABLED, or leave blank, to ignore the style and position information from your input captions and use default settings: white text with black outlining, bottom-center positioning, and automatic sizing. Whether you set Style passthrough to enabled or not, you can also choose to manually override any of the individual style and position settings.\"\n        }\n      ]\n    },\n    \"SubtitlingType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitlingType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"subtitlingType\"\n          },\n          \"description\": \"Specify whether your DVB subtitles\
  \ are standard or for hearing impaired. Choose hearing impaired if your subtitles include audio descriptions and dialogue. Choose standard if your subtitles include only dialogue.\"\n        }\n      ]\n    },\n    \"TeletextSpacing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DvbSubtitleTeletextSpacing\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"teletextSpacing\"\n          },\n          \"description\": \"Specify whether the Text spacing (TeletextSpacing) in your captions is set by the captions grid, or varies depending on letter width. Choose fixed grid (FIXED_GRID) to conform to the spacing specified in the captions file more accurately. Choose proportional (PROPORTIONAL) to make the text easier to read for closed captions. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"Width\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin1Max2147483647\"\
  \n        },\n        {\n          \"xml\": {\n            \"name\": \"width\"\n          },\n          \"description\": \"Specify the width, in pixels, of this set of DVB-Sub captions. The default value is 720 pixels. Related setting: When you use this setting, you must set DDS handling (ddsHandling) to a value other than None (NONE). All burn-in and DVB-Sub font settings must match.\"\n        }\n      ]\n    },\n    \"XPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"xPosition\"\n          },\n          \"description\": \"Specify the horizontal position (XPosition) of the captions, relative to the left side of the outputin pixels. A value of 10 would result in the captions starting 10 pixels from the left ofthe output. If no explicit x_position is provided, the horizontal caption position will bedetermined by the alignment parameter. Within your\
  \ job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    },\n    \"YPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integerMin0Max2147483647\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"yPosition\"\n          },\n          \"description\": \"Specify the vertical position (YPosition) of the captions, relative to the top of the output in pixels. A value of 10 would result in the captions starting 10 pixels from the top of the output. If no explicit y_position is provided, the caption will be positioned towards the bottom of the output. Within your job settings, all of your DVB-Sub settings must be identical.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-dvb-sub-destination-settings-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DvbSubDestinationSettings
---
