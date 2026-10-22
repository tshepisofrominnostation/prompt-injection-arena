# Prompt Injection Arena

An AI red-team QA tool: fires a 15-attack prompt-injection suite at simulated AI assistants and produces an evidence-backed security scorecard.

**Live prototype:** https://tshepisofrominnostation.github.io/prompt-injection-arena/
**Product brief:** see docs/BRIEF.md in this repo's wiki.

## What it demonstrates
- Five attack categories: direct injection, indirect injection (payloads hidden in documents/emails), jailbreaks, data exfiltration and instruction override.
- Verdict classification from responses: LEAKED / COMPROMISED / BLOCKED / PASSED, with the evidence for each.
- The defense-stack gap: run the suite with defenses OFF, then ON, and compare grades.
- Layered defense principles: input screening, instruction hardening, output filtering, least privilege.
- Mapping to the OWASP Top 10 for LLM Applications (LLM01, LLM02, LLM09).

## Principles
An LLM cannot reliably tell instructions from data, so anything a bot reads (documents, emails, web pages) is a potential attack channel. Defense is layered, never a single filter, and a security claim is only as good as its evidence.

## Use constraints
For QA and education, on systems you own or are authorised to test. Single-file vanilla HTML/JS with Tailwind CDN; everything runs client-side.

## Author
Tshepiso Freddy Thosago · portfolio: https://tshepisofrominnostation.github.io/portfolio/
