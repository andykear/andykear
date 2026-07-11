# FileMaker's undocumented XML, reverse engineered

FileMaker stores scripts, layouts, fields and tables as XML, but Claris has never published the format, and FileMaker's paste handler silently drops anything malformed. No error, the object just never appears.

I reverse engineered these formats through systematic round trip testing so that AI tools can generate FileMaker objects that actually paste. These repositories are that reference layer.

**[Script XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Claude-Skill)**
Makes AI generated scripts paste correctly. Full step ID dictionary and the hidden paste handler rules.

**[Layout XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Layout-Claude-Skill)**
Paste ready layout objects. All 18 object types, flags decoded, element order confirmed.

**[Field Definitions](https://github.com/andykear/FileMaker-XML-field-definitions)**
Field and table definition XML, verified down to auto enter, validation and calculation options.

**[XML Inspector](https://github.com/andykear/FileMaker-XML-inspector-open-source)**
Reads a Save as XML export in the browser. Finds unreferenced fields, broken references, diffs two versions.

**[XML Scrubber](https://github.com/andykear/FileMaker-XML-scrubber)**
Strips API keys, passwords and internal hostnames from FileMaker XML before you share it with an AI tool.

Everything is verified empirically, marked ✓ (round trip tested), ◎ (observed in exports) or ○ (inferred). All CC BY 4.0.

**Andrew Kear** · Claris Partner · Claris MVP · [clockworkct.co.uk](https://clockworkct.co.uk)
