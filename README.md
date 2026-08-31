# Speak Before the Reveal

**A method, and a tool for applying it: say your clinical reasoning aloud before
the AI scribe writes its version.**

An ambient AI scribe produces an excellent note and, in doing so, quietly takes
over the part of the work that made the clinician good at it. Reading a
plausible formulation is not the same cognitive act as producing one. Once you
have read the AI's impression, forming your own independently is much harder —
your judgement has already been anchored. Do that every day for a year and the
capacity degrades.

The remedy is order, not abstinence. Once the patient has left, keep recording
and dictate the reasoning before stopping the scribe. Spoken first, it is yours;
the scribe transcribes rather than invents, and the note carries the clinician's
thinking rather than a plausible reconstruction of it.

**The rule of thumb:** *if I have to think to produce it, I should say it.*

---

This repository takes one control from a broader governance paper — *speak
before the reveal*, the lowest-friction of seven proposed — and builds it out
into something a clinician can use tomorrow. The paper makes the wider argument
about workforce capability; this is the bedside end of it.

## What's in this repository

| | |
|---|---|
| [`skill/SKILL.md`](skill/SKILL.md) | An LLM skill that interviews a clinician and builds a cheat sheet for their own specialty and note type. Works in Claude, or pasted into a ChatGPT project. |
| [`cheatsheets/`](cheatsheets/) | Two worked examples — psychiatry and general medicine — as printable two-page reference guides. |

The psychiatry sheet is the exemplar. Supply it alongside `SKILL.md` and the
model has a layout to match.

## The mechanic

The skill does not tell a clinician which parts of their note to protect. It
asks them first, blind, and only then offers its own read for them to arbitrate.

That is the method applied to itself. A model that opens by listing the sections
it thinks matter produces exactly the artefact the paper warns about — a
plausible document the clinician edits rather than one they wrote. Structure,
vocabulary and formatting are safe for a model to propose. Identifying what
needs human authoring is not.

The interview then runs a second pass over whatever is left, looking for content
the scribe will supply **confidently and wrongly**. The distinction that matters:
omissions are safe, plausible completions are not. A blood pressure the scribe
never heard appears as a visible blank and you will notice. An examination
finding it never heard appears as a sentence that reads correctly and is untrue.

## Using it

**In Claude:** add `SKILL.md` as a skill, or paste it into a project's
instructions. Attach a cheat sheet from `cheatsheets/` as a formatting example.

**In ChatGPT:** paste the contents of `SKILL.md` into a Project's instructions
or a custom GPT, and upload a cheat sheet alongside.

Then ask it to build a cheat sheet for your specialty.

> **Do not paste patient information.** If you supply your note template, it
> must be blank. The skill is instructed to refuse completed notes, but the
> responsibility is yours.

The output is a printable sheet. It is meant to sit where you document, be used
for a fortnight, and then be revised against what you found. It is not finished
when the conversation ends.

## Scope and limits

This is a documentation-practice aid. It contains no thresholds, doses, decision
rules, scoring systems or diagnostic criteria, and it is designed not to
generate any — a cheat sheet that supplies clinical content is a scribe with
extra steps. The vocabulary it produces names findings you have already made.

Any sheet you build is yours. It has not been reviewed by the author of the
method, and every generated sheet carries a signature field for that reason.

## Credit

The underlying practice — continuing to narrate after the patient leaves —
originates with **Dr Michelle Adams**. The paper formalises it as *speak before
the reveal*; this repository extends it to other specialties.

## Citing this

The method:

> Jurblum M. *Speak Before the Reveal: Seven Solutions to Governing AI Scribe
> Deskilling Risk in Psychiatry and Mental Health Services.* Preprint,
> 28 July 2026. https://doi.org/10.2139/ssrn.7317778

The psychiatry cheat sheet: https://doi.org/10.5281/zenodo.22120151

This repository: see `CITATION.cff`, or the Zenodo DOI badge once the first
release is made.

## Contributing

Adaptations to other specialties are welcome — open an issue or a pull request
with the sheet and a note on what your specialty needed that the general
candidates missed. That feedback is the main way the skill's list of commonly
missing sections improves.

## Licence and disclaimer

[CC BY 4.0](LICENSE). Use it, adapt it, build on it — keep the attribution.

Please read [DISCLAIMER.md](DISCLAIMER.md) before using these materials. In
short: this is an aid to documentation practice and not clinical advice; any
cheat sheet you generate is your own clinical work and has not been reviewed by
the author; all AI output must be reviewed by the person who generated it; and
maintaining your own clinical templates and meeting your own medico-legal and
service documentation requirements remains your responsibility.
