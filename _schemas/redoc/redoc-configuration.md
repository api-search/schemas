---
description: Configuration options for ReDoc, the open-source API documentation renderer for OpenAPI specifications. These options control the functional behavior, appearance, and theme of the rendered documentation.
layout: schema
name: ReDoc Configuration
properties_list:
- description: Disables search indexing and hides the search box from the API documentation page.
  name: disableSearch
  type: boolean
- description: Sets the minimum number of characters that need to be typed into the search dialog to initiate the search.
  name: minCharacterLengthToInitSearch
  type: integer
- description: Hides the Download button for saving the API definition source file. This setting does not make the API definition private; it just hides the button.
  name: hideDownloadButtons
  type: boolean
- description: Hides the loading animation. Does not apply to CLI or Workflows-rendered docs.
  name: hideLoading
  type: boolean
- description: Hides the schema title next to the type.
  name: hideSchemaTitles
  type: boolean
- description: Sets the default expand level for JSON payload samples (response and request body). The default value is 2. Use 'all' to expand all levels.
  name: jsonSamplesExpandLevel
  type: object
- description: Displays only the specified number of enum values. Remaining values are hidden in an expandable area. If not set, all values are displayed.
  name: maxDisplayedEnumValues
  type: integer
- description: Shows only required fields in request samples.
  name: onlyRequiredInSamples
  type: boolean
- description: Shows required properties in schemas first, ordered in the same order as in the required array.
  name: sortRequiredPropsFirst
  type: boolean
- description: Specifies whether to automatically expand schemas in Reference docs. Set to 'all' to expand all schemas, or a number to expand schemas up to that level. Default is 0 (no expansion).
  name: schemasExpansionLevel
  type: object
- description: Specifies a vertical scroll-offset. Useful when fixed positioned elements (such as navbars or headers) are at the top of the page.
  name: scrollYOffset
  type: object
- description: Shows specification extensions (x- fields). Can be a boolean or an array of extension names.
  name: showExtensions
  type: object
- description: If set to true, the API definition is considered untrusted and all HTML/Markdown is sanitized to prevent XSS.
  name: sanitize
  type: boolean
- description: Set the URLs used to download the OpenAPI description or other documentation-related files from the API documentation page.
  name: downloadUrls
  type: array
- description: If a value is set, all schemas are rendered with the designated tag name and displayed in the sidebar navigation.
  name: schemaDefinitionsTagName
  type: string
- description: Controls how many schema levels are automatically generated for payload samples.
  name: generatedSamplesMaxDepth
  type: integer
- description: Enables hiding of parent names for nested properties within the documentation in complex data structures.
  name: hidePropertiesPrefix
  type: boolean
- description: Enables or disables expanding default server variables.
  name: expandDefaultServerVariables
  type: boolean
- description: Controls which responses to expand by default. Specify response codes as a comma-separated list (e.g. '200,201') or use 'all' to expand all.
  name: expandResponses
  type: object
- description: Automatically expands the single field in a schema.
  name: expandSingleSchemaField
  type: boolean
- description: If set to true, the protocol and hostname are not shown in the operation definition.
  name: hideHostname
  type: boolean
- description: Hides request payload examples.
  name: hideRequestPayloadSample
  type: boolean
- description: If set to true, the description for oneOf/anyOf objects is not shown in the schema.
  name: hideOneOfDescription
  type: boolean
- description: If set to true, the pattern is not shown in the schema.
  name: hideSchemaPattern
  type: boolean
- description: Hides the Security panel section.
  name: hideSecuritySection
  type: boolean
- description: Hides the request sample tab for requests with only one sample.
  name: hideSingleRequestSampleTab
  type: boolean
- description: If set to true, selecting an expanded item in the sidebar twice collapses it.
  name: menuToggle
  type: boolean
- description: If set to true, the sidebar uses the native scrollbar instead of perfect-scroll. A scrolling performance optimization for large API definitions.
  name: nativeScrollbars
  type: boolean
- description: Shows the path link and HTTP verb in the middle panel instead of the right panel.
  name: pathInMiddlePanel
  type: boolean
- description: If set, the payload sample is inserted at the specified index. Indexes start from 0.
  name: payloadSampleIdx
  type: integer
- description: Shows object schema example in the properties.
  name: showObjectSchemaExamples
  type: boolean
- description: When set to true, shows the HTTP request method for webhooks in operations and in the sidebar.
  name: showWebhookVerb
  type: boolean
- description: Shows only unique oneOf types in the label without titles.
  name: simpleOneOfTypeLabel
  type: boolean
- description: When set to true, sorts all enum values in all schemas alphabetically.
  name: sortEnumValuesAlphabetically
  type: boolean
- description: When set to true, sorts operations in the navigation sidebar and in the middle panel alphabetically.
  name: sortOperationsAlphabetically
  type: boolean
- description: When set to true, sorts properties in all schemas alphabetically.
  name: sortPropsAlphabetically
  type: boolean
- description: When set to true, sorts tags in the navigation sidebar and in the middle panel alphabetically.
  name: sortTagsAlphabetically
  type: boolean
- description: If set to true, the API definition is considered untrusted and all HTML/Markdown is sanitized to prevent XSS.
  name: untrustedSpec
  type: boolean
- description: Theme and visual styling options for the API documentation page.
  name: theme
  type: object
provider_name: ReDoc
provider_slug: redoc
schema_file: json-schema/redoc-configuration-schema.json
slug: redoc-configuration
source_filename: redoc-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://apievangelist.com/schemas/redoc/redoc-configuration.json\",\n  \"title\": \"ReDoc Configuration\",\n  \"description\": \"Configuration options for ReDoc, the open-source API documentation renderer for OpenAPI specifications. These options control the functional behavior, appearance, and theme of the rendered documentation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disableSearch\": {\n      \"type\": \"boolean\",\n      \"description\": \"Disables search indexing and hides the search box from the API documentation page.\",\n      \"default\": false\n    },\n    \"minCharacterLengthToInitSearch\": {\n      \"type\": \"integer\",\n      \"description\": \"Sets the minimum number of characters that need to be typed into the search dialog to initiate the search.\",\n      \"default\": 3,\n      \"minimum\": 1\n    },\n    \"hideDownloadButtons\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Hides the Download button for saving the API definition source file. This setting does not make the API definition private; it just hides the button.\",\n      \"default\": false\n    },\n    \"hideLoading\": {\n      \"type\": \"boolean\",\n      \"description\": \"Hides the loading animation. Does not apply to CLI or Workflows-rendered docs.\",\n      \"default\": false\n    },\n    \"hideSchemaTitles\": {\n      \"type\": \"boolean\",\n      \"description\": \"Hides the schema title next to the type.\",\n      \"default\": false\n    },\n    \"jsonSamplesExpandLevel\": {\n      \"oneOf\": [\n        {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"A numeric level to expand JSON payload samples to.\"\n        },\n        {\n          \"type\": \"string\",\n          \"enum\": [\"all\"],\n          \"description\": \"Expand all levels of JSON payload samples.\"\n        }\n      ],\n      \"description\": \"Sets the\
  \ default expand level for JSON payload samples (response and request body). The default value is 2. Use 'all' to expand all levels.\",\n      \"default\": 2\n    },\n    \"maxDisplayedEnumValues\": {\n      \"type\": \"integer\",\n      \"description\": \"Displays only the specified number of enum values. Remaining values are hidden in an expandable area. If not set, all values are displayed.\",\n      \"minimum\": 1\n    },\n    \"onlyRequiredInSamples\": {\n      \"type\": \"boolean\",\n      \"description\": \"Shows only required fields in request samples.\",\n      \"default\": false\n    },\n    \"sortRequiredPropsFirst\": {\n      \"type\": \"boolean\",\n      \"description\": \"Shows required properties in schemas first, ordered in the same order as in the required array.\",\n      \"default\": false\n    },\n    \"schemasExpansionLevel\": {\n      \"oneOf\": [\n        {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"A numeric level\
  \ to auto-expand schemas to.\"\n        },\n        {\n          \"type\": \"string\",\n          \"enum\": [\"all\"],\n          \"description\": \"Expand all schemas regardless of their level.\"\n        }\n      ],\n      \"description\": \"Specifies whether to automatically expand schemas in Reference docs. Set to 'all' to expand all schemas, or a number to expand schemas up to that level. Default is 0 (no expansion).\",\n      \"default\": 0\n    },\n    \"scrollYOffset\": {\n      \"oneOf\": [\n        {\n          \"type\": \"number\",\n          \"description\": \"A fixed number of pixels to be used as the vertical scroll offset.\"\n        },\n        {\n          \"type\": \"string\",\n          \"description\": \"A CSS selector for an element whose bottom edge defines the scroll offset.\"\n        }\n      ],\n      \"description\": \"Specifies a vertical scroll-offset. Useful when fixed positioned elements (such as navbars or headers) are at the top of the page.\"\n    },\n\
  \    \"showExtensions\": {\n      \"oneOf\": [\n        {\n          \"type\": \"boolean\",\n          \"description\": \"When true, shows all specification extensions (x- fields). Extensions used by Redoc are ignored.\"\n        },\n        {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"An array of extension names to selectively display.\"\n        }\n      ],\n      \"description\": \"Shows specification extensions (x- fields). Can be a boolean or an array of extension names.\",\n      \"default\": false\n    },\n    \"sanitize\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the API definition is considered untrusted and all HTML/Markdown is sanitized to prevent XSS.\",\n      \"default\": false\n    },\n    \"downloadUrls\": {\n      \"type\": \"array\",\n      \"description\": \"Set the URLs used to download the OpenAPI description or other documentation-related files\
  \ from the API documentation page.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DownloadUrl\"\n      }\n    },\n    \"schemaDefinitionsTagName\": {\n      \"type\": \"string\",\n      \"description\": \"If a value is set, all schemas are rendered with the designated tag name and displayed in the sidebar navigation.\",\n      \"minLength\": 1\n    },\n    \"generatedSamplesMaxDepth\": {\n      \"type\": \"integer\",\n      \"description\": \"Controls how many schema levels are automatically generated for payload samples.\",\n      \"default\": 8,\n      \"minimum\": 1\n    },\n    \"hidePropertiesPrefix\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enables hiding of parent names for nested properties within the documentation in complex data structures.\",\n      \"default\": true\n    },\n    \"expandDefaultServerVariables\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enables or disables expanding default server variables.\",\n      \"default\": false\n\
  \    },\n    \"expandResponses\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"pattern\": \"^(all|[0-9]+(,[0-9]+)*)$\",\n          \"description\": \"Comma-separated HTTP response codes to expand, or 'all' to expand all responses.\"\n        }\n      ],\n      \"description\": \"Controls which responses to expand by default. Specify response codes as a comma-separated list (e.g. '200,201') or use 'all' to expand all.\"\n    },\n    \"expandSingleSchemaField\": {\n      \"type\": \"boolean\",\n      \"description\": \"Automatically expands the single field in a schema.\",\n      \"default\": false\n    },\n    \"hideHostname\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the protocol and hostname are not shown in the operation definition.\",\n      \"default\": false\n    },\n    \"hideRequestPayloadSample\": {\n      \"type\": \"boolean\",\n      \"description\": \"Hides request payload examples.\",\n      \"default\": false\n\
  \    },\n    \"hideOneOfDescription\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the description for oneOf/anyOf objects is not shown in the schema.\",\n      \"default\": false\n    },\n    \"hideSchemaPattern\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the pattern is not shown in the schema.\",\n      \"default\": false\n    },\n    \"hideSecuritySection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Hides the Security panel section.\",\n      \"default\": false\n    },\n    \"hideSingleRequestSampleTab\": {\n      \"type\": \"boolean\",\n      \"description\": \"Hides the request sample tab for requests with only one sample.\",\n      \"default\": false\n    },\n    \"menuToggle\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, selecting an expanded item in the sidebar twice collapses it.\",\n      \"default\": true\n    },\n    \"nativeScrollbars\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"If set to true, the sidebar uses the native scrollbar instead of perfect-scroll. A scrolling performance optimization for large API definitions.\",\n      \"default\": false\n    },\n    \"pathInMiddlePanel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Shows the path link and HTTP verb in the middle panel instead of the right panel.\",\n      \"default\": false\n    },\n    \"payloadSampleIdx\": {\n      \"type\": \"integer\",\n      \"description\": \"If set, the payload sample is inserted at the specified index. Indexes start from 0.\",\n      \"minimum\": 0\n    },\n    \"showObjectSchemaExamples\": {\n      \"type\": \"boolean\",\n      \"description\": \"Shows object schema example in the properties.\",\n      \"default\": false\n    },\n    \"showWebhookVerb\": {\n      \"type\": \"boolean\",\n      \"description\": \"When set to true, shows the HTTP request method for webhooks in operations and in the sidebar.\",\n      \"default\": false\n\
  \    },\n    \"simpleOneOfTypeLabel\": {\n      \"type\": \"boolean\",\n      \"description\": \"Shows only unique oneOf types in the label without titles.\",\n      \"default\": false\n    },\n    \"sortEnumValuesAlphabetically\": {\n      \"type\": \"boolean\",\n      \"description\": \"When set to true, sorts all enum values in all schemas alphabetically.\",\n      \"default\": false\n    },\n    \"sortOperationsAlphabetically\": {\n      \"type\": \"boolean\",\n      \"description\": \"When set to true, sorts operations in the navigation sidebar and in the middle panel alphabetically.\",\n      \"default\": false\n    },\n    \"sortPropsAlphabetically\": {\n      \"type\": \"boolean\",\n      \"description\": \"When set to true, sorts properties in all schemas alphabetically.\",\n      \"default\": false\n    },\n    \"sortTagsAlphabetically\": {\n      \"type\": \"boolean\",\n      \"description\": \"When set to true, sorts tags in the navigation sidebar and in the middle panel alphabetically.\"\
  ,\n      \"default\": false\n    },\n    \"untrustedSpec\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set to true, the API definition is considered untrusted and all HTML/Markdown is sanitized to prevent XSS.\",\n      \"default\": false\n    },\n    \"theme\": {\n      \"$ref\": \"#/$defs/ThemeOptions\",\n      \"description\": \"Theme and visual styling options for the API documentation page.\"\n    }\n  },\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"DownloadUrl\": {\n      \"type\": \"object\",\n      \"description\": \"A URL entry for downloading an OpenAPI description or related documentation file.\",\n      \"required\": [\"url\"],\n      \"properties\": {\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL pointing to the downloadable file.\"\n        },\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable label for the download\
  \ link.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"ThemeOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Visual theme configuration for the Redoc documentation renderer.\",\n      \"properties\": {\n        \"spacing\": {\n          \"$ref\": \"#/$defs/SpacingOptions\",\n          \"description\": \"Spacing and padding settings used in the layout.\"\n        },\n        \"breakpoints\": {\n          \"$ref\": \"#/$defs/BreakpointOptions\",\n          \"description\": \"Breakpoints for switching between three-panel, two-panel, and mobile view layouts.\"\n        },\n        \"colors\": {\n          \"$ref\": \"#/$defs/ColorOptions\",\n          \"description\": \"Color settings including tonal offset and primary/secondary palette.\"\n        },\n        \"typography\": {\n          \"$ref\": \"#/$defs/TypographyOptions\",\n          \"description\": \"Typography settings including font family, size, weight, and line height.\"\n      \
  \  },\n        \"sidebar\": {\n          \"$ref\": \"#/$defs/SidebarOptions\",\n          \"description\": \"Sidebar width, background color, text color, and item styling.\"\n        },\n        \"logo\": {\n          \"$ref\": \"#/$defs/LogoOptions\",\n          \"description\": \"Logo display settings including max dimensions and padding.\"\n        },\n        \"rightPanel\": {\n          \"$ref\": \"#/$defs/RightPanelOptions\",\n          \"description\": \"Right panel background color, width, text color, and server display options.\"\n        },\n        \"fab\": {\n          \"$ref\": \"#/$defs/FabOptions\",\n          \"description\": \"Floating action button (FAB) styling.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"SpacingOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Spacing configuration for the Redoc layout.\",\n      \"properties\": {\n        \"unit\": {\n          \"type\": \"integer\",\n          \"description\": \"\
  Main spacing unit (in pixels) used in auto-computed theme values.\",\n          \"default\": 5\n        },\n        \"sectionHorizontal\": {\n          \"type\": \"integer\",\n          \"description\": \"Horizontal section padding in pixels. Defaults to spacing.unit * 8.\",\n          \"default\": 40\n        },\n        \"sectionVertical\": {\n          \"type\": \"integer\",\n          \"description\": \"Vertical section padding in pixels. Defaults to spacing.unit * 8.\",\n          \"default\": 40\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"BreakpointOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Responsive breakpoints for layout switching.\",\n      \"properties\": {\n        \"small\": {\n          \"type\": \"string\",\n          \"description\": \"Breakpoint for switching to mobile view.\",\n          \"default\": \"50rem\"\n        },\n        \"medium\": {\n          \"type\": \"string\",\n          \"description\": \"Breakpoint\
  \ for switching to two-panel view.\",\n          \"default\": \"85rem\"\n        },\n        \"large\": {\n          \"type\": \"string\",\n          \"description\": \"Breakpoint for switching to three-panel view.\",\n          \"default\": \"105rem\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"ColorOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Color palette settings for the Redoc theme.\",\n      \"properties\": {\n        \"tonalOffset\": {\n          \"type\": \"number\",\n          \"description\": \"Default tonal offset used in color computations.\",\n          \"default\": 0.3,\n          \"minimum\": 0,\n          \"maximum\": 1\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"TypographyOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Typography settings for the Redoc documentation.\",\n      \"properties\": {\n        \"fontSize\": {\n          \"type\": \"string\",\n          \"\
  description\": \"Base font size for body text.\",\n          \"default\": \"14px\"\n        },\n        \"lineHeight\": {\n          \"type\": \"string\",\n          \"description\": \"Base line height for body text.\",\n          \"default\": \"1.5em\"\n        },\n        \"fontWeightRegular\": {\n          \"type\": \"string\",\n          \"description\": \"Font weight for regular text.\",\n          \"default\": \"400\"\n        },\n        \"fontWeightBold\": {\n          \"type\": \"string\",\n          \"description\": \"Font weight for bold text.\",\n          \"default\": \"600\"\n        },\n        \"fontWeightLight\": {\n          \"type\": \"string\",\n          \"description\": \"Font weight for light text.\",\n          \"default\": \"300\"\n        },\n        \"fontFamily\": {\n          \"type\": \"string\",\n          \"description\": \"Font family for body text.\",\n          \"default\": \"Roboto, sans-serif\"\n        },\n        \"smoothing\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Font smoothing setting.\",\n          \"default\": \"antialiased\"\n        },\n        \"optimizeSpeed\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to optimize text rendering for speed.\",\n          \"default\": true\n        },\n        \"headings\": {\n          \"$ref\": \"#/$defs/HeadingTypographyOptions\",\n          \"description\": \"Typography settings specific to headings.\"\n        },\n        \"code\": {\n          \"$ref\": \"#/$defs/CodeTypographyOptions\",\n          \"description\": \"Typography settings for inline code blocks.\"\n        },\n        \"links\": {\n          \"$ref\": \"#/$defs/LinkTypographyOptions\",\n          \"description\": \"Typography settings for hyperlinks.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"HeadingTypographyOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Typography settings for headings.\",\n      \"properties\"\
  : {\n        \"fontFamily\": {\n          \"type\": \"string\",\n          \"description\": \"Font family for headings.\",\n          \"default\": \"Montserrat, sans-serif\"\n        },\n        \"fontWeight\": {\n          \"type\": \"string\",\n          \"description\": \"Font weight for headings.\",\n          \"default\": \"400\"\n        },\n        \"lineHeight\": {\n          \"type\": \"string\",\n          \"description\": \"Line height for headings.\",\n          \"default\": \"1.6em\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"CodeTypographyOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Typography settings for inline code.\",\n      \"properties\": {\n        \"fontSize\": {\n          \"type\": \"string\",\n          \"description\": \"Font size for inline code.\",\n          \"default\": \"13px\"\n        },\n        \"fontFamily\": {\n          \"type\": \"string\",\n          \"description\": \"Font family for inline\
  \ code.\",\n          \"default\": \"Courier, monospace\"\n        },\n        \"fontWeight\": {\n          \"type\": \"string\",\n          \"description\": \"Font weight for inline code.\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"Text color for inline code.\",\n          \"default\": \"#e53935\"\n        },\n        \"backgroundColor\": {\n          \"type\": \"string\",\n          \"description\": \"Background color for inline code.\",\n          \"default\": \"rgba(38, 50, 56, 0.05)\"\n        },\n        \"wrap\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to break word for inline blocks (otherwise they can overflow).\",\n          \"default\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"LinkTypographyOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Typography and color settings for hyperlinks.\",\n      \"properties\": {\n        \"color\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Link text color. Defaults to the primary color.\"\n        },\n        \"visited\": {\n          \"type\": \"string\",\n          \"description\": \"Visited link color. Defaults to the link color.\"\n        },\n        \"hover\": {\n          \"type\": \"string\",\n          \"description\": \"Hover link color. Defaults to a lightened version of the link color.\"\n        },\n        \"textDecoration\": {\n          \"type\": \"string\",\n          \"description\": \"CSS text-decoration for links.\",\n          \"default\": \"auto\"\n        },\n        \"hoverTextDecoration\": {\n          \"type\": \"string\",\n          \"description\": \"CSS text-decoration for links on hover.\",\n          \"default\": \"auto\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"SidebarOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Styling and layout options for the navigation sidebar.\"\
  ,\n      \"properties\": {\n        \"width\": {\n          \"type\": \"string\",\n          \"description\": \"Width of the sidebar.\",\n          \"default\": \"260px\"\n        },\n        \"backgroundColor\": {\n          \"type\": \"string\",\n          \"description\": \"Background color of the sidebar.\",\n          \"default\": \"#fafafa\"\n        },\n        \"textColor\": {\n          \"type\": \"string\",\n          \"description\": \"Text color in the sidebar.\",\n          \"default\": \"#333333\"\n        },\n        \"activeTextColor\": {\n          \"type\": \"string\",\n          \"description\": \"Text color for the active sidebar item. Defaults to the primary color.\"\n        },\n        \"groupItems\": {\n          \"$ref\": \"#/$defs/SidebarItemOptions\",\n          \"description\": \"Styling for group heading items in the sidebar.\"\n        },\n        \"level1Items\": {\n          \"$ref\": \"#/$defs/SidebarItemOptions\",\n          \"description\": \"Styling\
  \ for level 1 sidebar items such as tags and section headings.\"\n        },\n        \"arrow\": {\n          \"$ref\": \"#/$defs/SidebarArrowOptions\",\n          \"description\": \"Styling for the sidebar expand/collapse arrow.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"SidebarItemOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Styling for a category of sidebar items.\",\n      \"properties\": {\n        \"activeBackgroundColor\": {\n          \"type\": \"string\",\n          \"description\": \"Background color for the active state of this sidebar item group.\"\n        },\n        \"activeTextColor\": {\n          \"type\": \"string\",\n          \"description\": \"Text color for the active state of this sidebar item group.\"\n        },\n        \"textTransform\": {\n          \"type\": \"string\",\n          \"description\": \"CSS text-transform for sidebar item labels.\",\n          \"enum\": [\"uppercase\", \"lowercase\", \"\
  capitalize\", \"none\"],\n          \"default\": \"none\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"SidebarArrowOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Styling for the sidebar navigation arrow icon.\",\n      \"properties\": {\n        \"size\": {\n          \"type\": \"string\",\n          \"description\": \"Size of the arrow icon.\",\n          \"default\": \"1.5em\"\n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"Color of the arrow icon. Defaults to the sidebar text color.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"LogoOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Display settings for the logo shown above the sidebar.\",\n      \"properties\": {\n        \"maxHeight\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum height of the logo image. Defaults to the sidebar width.\"\n        },\n       \
  \ \"maxWidth\": {\n          \"type\": \"string\",\n          \"description\": \"Maximum width of the logo image. Defaults to the sidebar width.\"\n        },\n        \"gutter\": {\n          \"type\": \"string\",\n          \"description\": \"Padding around the logo image.\",\n          \"default\": \"2px\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"RightPanelOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Styling options for the right panel, which shows request and response examples.\",\n      \"properties\": {\n        \"backgroundColor\": {\n          \"type\": \"string\",\n          \"description\": \"Background color of the right panel.\",\n          \"default\": \"#263238\"\n        },\n        \"width\": {\n          \"type\": \"string\",\n          \"description\": \"Width of the right panel as a percentage or CSS value.\",\n          \"default\": \"40%\"\n        },\n        \"textColor\": {\n          \"type\": \"string\"\
  ,\n          \"description\": \"Text color in the right panel.\",\n          \"default\": \"#ffffff\"\n        },\n        \"servers\": {\n          \"$ref\": \"#/$defs/RightPanelServersOptions\",\n          \"description\": \"Server selector overlay styling in the right panel.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"RightPanelServersOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Styling for the server selector display in the right panel.\",\n      \"properties\": {\n        \"overlay\": {\n          \"type\": \"object\",\n          \"description\": \"Overlay styling for the server selector.\",\n          \"properties\": {\n            \"backgroundColor\": {\n              \"type\": \"string\",\n              \"description\": \"Background color of the server selector overlay.\",\n              \"default\": \"#fafafa\"\n            },\n            \"textColor\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Text color in the server selector overlay.\",\n              \"default\": \"#263238\"\n            }\n          },\n          \"additionalProperties\": false\n        },\n        \"url\": {\n          \"type\": \"object\",\n          \"description\": \"URL display styling in the server selector.\",\n          \"properties\": {\n            \"backgroundColor\": {\n              \"type\": \"string\",\n              \"description\": \"Background color for the server URL display.\",\n              \"default\": \"#fff\"\n            }\n          },\n          \"additionalProperties\": false\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"FabOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Styling options for the floating action button.\",\n      \"properties\": {\n        \"backgroundColor\": {\n          \"type\": \"string\",\n          \"description\": \"Background color of the floating action button.\",\n          \"default\": \"#263238\"\
  \n        },\n        \"color\": {\n          \"type\": \"string\",\n          \"description\": \"Icon color of the floating action button.\",\n          \"default\": \"#ffffff\"\n        }\n      },\n      \"additionalProperties\": false\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/redoc/refs/heads/main/json-schema/redoc-configuration-schema.json
tags:
- API Documentation
- Developer Tools
- Documentation
- OpenAPI
- Reference
- Renderer
title: ReDoc Configuration
---
