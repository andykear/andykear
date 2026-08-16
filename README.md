## Analyse a FileMaker solution in your browser
Nothing installed, nothing uploaded, works offline.

**[Clockwork Inspector](https://github.com/andykear/FileMaker-XML-inspector-open-source)** (SaXML)
Drop in a Save as XML export. Unreferenced fields tiered by confidence, broken references, script call tree, relationship graph drawn from the real TO geometry, layout wireframes, and a diff between two versions down to the calculation line.
Every check is documented, so the findings are defensible in front of a client.

**[XML Scrubber](https://github.com/andykear/FileMaker-XML-scrubber)** (SaXML + others)
Strips API keys, passwords and internal hostnames out of FileMaker XML before you hand it to an AI tool.

## Reliable AI for FileMaker

AI is genuinely useful for FileMaker development, but only if it stops guessing. Left to its training data, a model invents functions that don't exist, and emits layout and schema XML that FileMaker rejects silently — no error, the object just never appears.

These are open tools and specifications that fix that: the knowledge an AI needs to generate FileMaker that actually works, and the tools to check what it produces. Much of it is reverse-engineering FileMaker's undocumented clipboard XML — the formats Claris has never published, where a wrong guess pastes silently and breaks. The rest is giving the model the vocabulary and verification it otherwise lacks.

**Start here**

**[FileMaker Second Opinion](https://github.com/andykear/FileMaker-second-opinion)**
A reasoning skill, not a knowledge file. It makes the model challenge its own first answer on exactly the problems where the common FileMaker solution works in a demo and fails silently in production, and it forces a proper read of Claris Help, Notes and platform sections included, before any behaviour claim is made. Built and refined against production work. New, and the piece the rest of this page stacks under.

**[FileMaker AI Vocabulary](https://github.com/andykear/FileMaker-AI-vocabulary)**
Every FileMaker 26 function and script step in ~7,000 tokens, so an AI stops inventing things that don't exist. The cheapest way to make any model better at FileMaker — no XML required.

**Generation — paste-ready FileMaker XML**

**[Script XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Claude-Skill)** (XMSS, XMSC, XMFN)
The full script step ID dictionary, plus the hidden paste-handler rules that decide whether your XML survives the trip into FileMaker.

**[Layout XML Skill](https://github.com/andykear/FileMaker-XMLsnippet-Layout-Claude-Skill)** (XML2)
All 18 layout object types mapped, every flag decoded, element order confirmed against native output. Verified across 45+ layouts in 10 production files.

**[Field, Table & Value List Definitions](https://github.com/andykear/FileMaker-XML-field-definitions)** (XMFD, XMTB, XMVL)
Field, table and value list definition XML — auto-enter, validation, storage, calculation options, and the three value list source arms — verified down to the individual option level.

**Verified, not guessed**

Every finding here is marked so you know exactly how sure I am:
✓ round-trip tested · ◎ observed in native exports · ○ inferred

All CC BY 4.0.

Andrew Kear · Claris Partner · Claris MVP · [clockworkct.co.uk](https://clockworkct.co.uk)
