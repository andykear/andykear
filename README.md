# FileMaker's undocumented XML, reverse engineered

FileMaker stores scripts, layouts, fields and tables as XML — but Claris has never published the format, and FileMaker's paste handler silently drops anything it doesn't like. No error. The object just never appears.

I reverse engineered these formats to build a reference layer for agentic development.

This work now powers two kinds of tool: skills that let AI generate FileMaker objects which actually paste, and standalone tools that analyse Save as XML exports and clean XML directly with no AI required.

**Generation — paste-ready FileMaker**

**[Script XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Claude-Skill)**
The full script step ID dictionary, plus the hidden paste-handler rules that decide whether your XML survives the trip into FileMaker.

**[Layout XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Layout-Claude-Skill)**
All 18 layout object types mapped, every flag decoded, element order confirmed against native output. Verified across 45+ layouts in 10 production files.

**[Field Definitions](https://github.com/andykear/FileMaker-XML-field-definitions)**
Field and table definition XML — auto-enter, validation, storage and calculation options — verified down to the individual option level.

**Analysis — read, audit and clean existing XML**

**[XML Inspector](https://github.com/andykear/FileMaker-XML-inspector-open-source)**
Full-catalog dependency analysis of a Save as XML export, entirely in the browser. Finds unreferenced fields, silent-failure risks, broken references, and diffs two versions of a solution against each other.

**[XML Scrubber](https://github.com/andykear/FileMaker-XML-scrubber)**
Strips API keys, passwords and internal hostnames out of FileMaker XML before you hand it to an AI tool.

**Verified, not guessed**

Every finding here is marked so you know exactly how sure I am:
✓ round-trip tested · ◎ observed in native exports · ○ inferred

All CC BY 4.0.

Andrew Kear · Claris Partner · Claris MVP · [clockworkct.co.uk](https://clockworkct.co.uk)
