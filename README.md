# Speak Before the Reveal

**Say your clinical reasoning out loud before the AI scribe writes its version.**

An ambient scribe produces an excellent note, and while it is doing that it
offers to quietly take over the part of the work that is critical to doing your 
job safely. Reading a plausible clinical synthesis is not the same cognitive act as 
producing one. Once you have read the model's impression, forming your own 
gets harder as your judgement has already been anchored to it. Do that every 
day for a year and see what happens to the capacity.

This is what happened to all of us with Google Maps and navigating our own
streets. The tool was better at the task, so we stopped doing the task, and then
we stopped being able to.

The fix is sequence, not abstinence. Once the patient has left, keep recording and
dictate the reasoning before you stop the scribe. Said first, you practice the 
skill and the output is yours. The scribe transcribes it instead of inventing it, 
and the note carries your thinking rather than a plausible reconstruction of it.

The rule of thumb: **if I have to think to produce it, I should say it.**

This repository takes one control out of a broader governance paper, speak
before the reveal, and builds it into something a clinician from any healthcare
specialty can use tomorrow. The paper makes the wider argument about workforce 
capability. The skill is the first practical tool to emerge from it.

## What's in here

- [`skill/SKILL.md`](skill/SKILL.md), an LLM skill that interviews a clinician
  and builds a reference guide for their own specialty and note type. Works as a
  Claude or ChatGPT skill. 
- [`cheatsheets/`](cheatsheets/), three worked examples, psychiatry, general
  medicine and general practice, as printable two-page guides. These are examples 
  of what the output should look like.

The psychiatry sheet is the exemplar. Hand it to the model alongside `SKILL.md`
and it has a layout to copy.

## Why it asks you first

The skill does not tell a clinician which parts of their note to protect. It
asks them first, blind, and only then offers its own read for them to arbitrate.

That is the method applied to itself. A model that opens by listing the sections
it thinks matter hands you exactly the artefact the paper warns about, a
plausible document you edit rather than one you wrote. Structure, vocabulary and
formatting are safe for a model to propose. Working out what needs a human
author is not.

The interview then runs a second pass over whatever is left, hunting for the
content a scribe will supply **confidently and wrongly**. The distinction that
matters is that omissions are safe and plausible completions are not. A blood
pressure the scribe never heard turns up as a blank and you notice it. That's **safe**. An
examination finding it never heard turns up as a sentence that reads correctly
and is untrue and therefore **dangerous**.

## Using it

It is designed to work in both Claude and ChatGPT. Testing across the two is
ongoing, so if it behaves differently in one of them, that is worth an issue.

In both Claude and ChatGPT, add `SKILL.md` as a skill, or paste it into a new 
conversation. You can also attach one of the cheat sheets from `cheatsheets/` 
as a formatting example.

Then ask it to build a guide for your specialty.

> **Don't paste patient information.** If you give it your note template, the
> template has to be blank. The skill is instructed to refuse completed notes,
> but that is a safeguard, not a guarantee, and the responsibility is yours.

What comes out is a Word document, which you can export as a PDF if you want one. 
Word first, on purpose, because you will want to change it. Print it, keep it 
where you document, use it for a fortnight, then come back and revise it against 
what you actually found. It isn't finished when the conversation ends.

## Scope and limits

This is an aid to remind you what to say to the scribe to build up good documentation 
practice. There are no thresholds, doses, decision rules, scoring systems or diagnostic 
criteria in it, and the skill is built not to generate any, because a cheat sheet that 
supplies clinical content is a scribe with extra steps. The vocabulary it gives you are 
cues to help you think more broadly through your spoken synthesis.

The method is a reasoned precaution and has not been evaluated in a trial. The
rationale comes from adjacent evidence on automation bias and skill decay, not
from a study of AI scribes and clinical reasoning, because that study does not
exist (yet).

Any sheet you build is yours. I have not reviewed it, which is why every
generated sheet carries a signature field.

## Credit

The underlying practice, continuing to narrate after the patient leaves,
originates with **Dr Michelle Adams of Time to Grow Clinic**. The paper formalises it 
as *speak before the reveal*, and this repository extends it to other specialties.

Thank you also to **Dr Rob Selzer** for his input in developing the original paper.

## Citing this

The method:

> Jurblum M. *Speak Before the Reveal: Seven Solutions to Governing AI Scribe
> Deskilling Risk in Psychiatry and Mental Health Services.* Preprint,
> 28 July 2026. https://doi.org/10.2139/ssrn.7317778

The psychiatry cheat sheet: https://doi.org/10.5281/zenodo.22120151

This repository: see `CITATION.cff`, or the Zenodo DOI badge once the first
release is made.

## Contributing

Adaptations to other specialties are welcome. Open an issue or a pull request
with the sheet, and say what your specialty needed that the general candidates
missed. That feedback is the main way the skill's list of commonly missing
sections improves.

## Licence and disclaimer

[CC BY 4.0](LICENSE). Use it, adapt it, build on it, keep the attribution.

Read [DISCLAIMER.md](DISCLAIMER.md) before you use any of this. It covers what
this is not: not clinical advice, not reviewed by me, and not a substitute for
maintaining your own templates or meeting your own documentation requirements.
