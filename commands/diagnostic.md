---
description: Start a YAID diagnostic for a supported Claude certification and identify study priorities.
argument-hint: "[ccar-f | ccdv-f | ccao-f | ccar-p]"
---

Help the learner start a diagnostic with YAID's declared MCP tools. The requested track is: $ARGUMENTS

Read the certification-coach skill, then call certification_catalog. If the argument is missing or not a supported exam code, clarify the learner's intended work and choose from the catalog. Start diagnostic mode and present the first question. On a host with interactive MCP Apps, show the practice card. Otherwise show the returned options in text and wait for the learner's selection. Do not submit an answer for them, reveal assessment explanations early, or report a practice score as official exam readiness.
