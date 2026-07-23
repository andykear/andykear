# Reliable AI for FileMaker

AI is genuinely useful for FileMaker development, but only if it stops guessing. Left to its training data, a model invents functions that don't exist, and emits layout and schema XML that FileMaker rejects silently — no error, the object just never appears.

These are open tools and specifications that fix that: the knowledge an AI needs to generate FileMaker that actually works, and the tools to check what it produces. Much of it is reverse-engineering FileMaker's undocumented clipboard XML — the formats Claris has never published, where a wrong guess pastes silently and breaks. The rest is giving the model the vocabulary and verification it otherwise lacks.

**Start here**

**[FileMaker AI Vocabulary](https://github.com/andykear/FileMaker-AI-vocabulary)**
Every FileMaker 26 function and script step in ~7,000 tokens, so an AI stops inventing things that don't exist. The cheapest way to make any model better at FileMaker — no XML required.

**Generation — paste-ready FileMaker XML**

**[Script XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Claude-Skill)** (XMSS, XMSC, XMFN)
The full script step ID dictionary, plus the hidden paste-handler rules that decide whether your XML survives the trip into FileMaker.

**[Layout XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Layout-Claude-Skill)** (XML2)
All 18 layout object types mapped, every flag decoded, element order confirmed against native output. Verified across 45+ layouts in 10 production files.

**[Field, Table & Value List Definitions](https://github.com/andykear/FileMaker-XML-field-definitions)** (XMFD, XMTB, XMVL)
Field, table and value list definition XML — auto-enter, validation, storage, calculation options, and the three value list source arms — verified down to the individual option level.

**Analysis — read, audit and clean existing XML**

**[XML Inspector](https://github.com/andykear/FileMaker-XML-inspector-open-source)** (SaXML)
Full-catalog dependency analysis of a Save as XML export, entirely in the browser. Finds unreferenced fields, silent-failure risks, broken references, and diffs two versions of a solution against each other.

**[XML Scrubber](https://github.com/andykear/FileMaker-XML-scrubber)** (SaXML + others)
Strips API keys, passwords and internal hostnames out of FileMaker XML before you hand it to an AI tool.

**Verified, not guessed**

Every finding here is marked so you know exactly how sure I am:
✓ round-trip tested · ◎ observed in native exports · ○ inferred

All CC BY 4.0.

Andrew Kear · Claris Partner · Claris MVP · [clockworkct.co.uk](https://clockworkct.co.uk)
