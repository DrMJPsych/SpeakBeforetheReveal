# Speak Before the Reveal

One-page reference guides that help you keep your clinical reasoning your own
when you use an AI scribe. Free to download and use. No account, no login,
nothing to install.

## Download a guide

Pick your specialty. The PDF is ready to print. The Word file is there if you
want to change the wording to suit how you work.

| Specialty | Print it | Edit it |
|---|---|---|
| Psychiatry | [PDF](https://github.com/DrMJPsych/SpeakBeforetheReveal/raw/main/guides/Speak_Before_the_Reveal_Psychiatry.pdf) | [Word](https://github.com/DrMJPsych/SpeakBeforetheReveal/raw/main/guides/Speak_Before_the_Reveal_Psychiatry.docx) |
| General medicine | [PDF](https://github.com/DrMJPsych/SpeakBeforetheReveal/raw/main/guides/Speak_Before_the_Reveal_General_Medicine.pdf) | [Word](https://github.com/DrMJPsych/SpeakBeforetheReveal/raw/main/guides/Speak_Before_the_Reveal_General_Medicine.docx) |
| General practice | [PDF](https://github.com/DrMJPsych/SpeakBeforetheReveal/raw/main/guides/Speak_Before_the_Reveal_General_Practice.pdf) | [Word](https://github.com/DrMJPsych/SpeakBeforetheReveal/raw/main/guides/Speak_Before_the_Reveal_General_Practice.docx) |

The psychiatry guide is mine and I use it. The general medicine and general
practice guides are examples built by a psychiatrist and need review by someone
who does that work.

## How to use it

Print it and keep it where you document. When the patient has left, keep the
scribe recording and say your reasoning out loud before you stop it. Impression,
risk, plan, and why. Then stop the recording and read what it wrote.

The rule of thumb: **if I have to think to produce it, I should say it.**

That is the whole intervention. It takes about a minute and works with any
scribe software.

## Make one for your own specialty

There is a file here that does the work for you. It interviews you about your
specialty, your note template and how you actually work, then writes your guide.

1. Open [`skill/SKILL.md`](skill/SKILL.md) and click the copy icon at the top
   right of the file. Read it before you run it. That is good practice with
   anything you hand to an AI, and it is a fair test of whether you trust what
   it is going to ask you.
2. Start a new conversation in ChatGPT, Claude or Gemini.
3. Paste the whole thing in, attach one of the guides above so it has a layout
   to copy, and ask it to build a guide for your specialty.
4. It will ask you questions before it writes anything. Answer them properly.
   That is the point. A guide you edited is not the same as a guide you wrote.

You get a Word document out. Export it to PDF once you are happy with it.

> **Do not paste patient information.** If you give it your note template, the
> template has to be blank. The file is written to refuse completed notes, but
> that is a safeguard, not a guarantee, and the responsibility is yours.

## Send me yours

If you build a guide for general practice, nursing, emergency, surgery,
paediatrics or allied health, get in touch on LinkedIn and I will add it here
with your name on it. A pool of guides across specialties is worth a good deal
more than one psychiatrist's version.

Please send the text rather than the file. I will rebuild the document at this
end. Nobody should be opening attachments from strangers, and that applies to me
as much as to you.

Tell me what your specialty needed that the guide did not prompt for. That
feedback is the main way this improves.

## Why this exists

An ambient scribe produces an excellent note, and while it is doing that it
offers to quietly take over the part of the work that is critical to doing your
job safely. Reading a plausible clinical synthesis is not the same cognitive act
as producing one. Once you have read the model's impression, forming your own
gets harder as your judgement has already been anchored to it. Do that every day
for a year and see what happens to the capacity.

This is what happened to all of us with Google Maps and navigating our own
streets. The tool was better at the task, so we stopped doing the task, and then
we stopped being able to.

The fix is sequence, not abstinence. Said first, you practise the skill and the
output is yours. The scribe transcribes your reasoning instead of inventing its
own.

This repository takes one control out of a broader governance paper, speak
before the reveal, and builds it into something a clinician from any healthcare
specialty can use tomorrow. The paper makes the wider argument about workforce
capability. This is the practical end of it.

## Why the guide interviews you first

It does not tell you which parts of your note to protect. It asks you first,
blind, and only then offers its own read for you to arbitrate.

That is the method applied to itself. A model that opens by listing the sections
it thinks matter hands you exactly the artefact the paper warns about, a
plausible document you edit rather than one you wrote.

It then runs a second pass looking for what a scribe will supply **confidently
and wrongly**. A blood pressure it never heard turns up as a blank and you
notice it. That is **safe**. An examination finding it never heard turns up as a
sentence that reads correctly and is untrue, and that is **dangerous**.

## Scope and limits

This is an aid to remind you what to say to the scribe. There are no thresholds,
doses, decision rules, scoring systems or diagnostic criteria in it, and it is
built not to generate any, because a guide that supplies clinical content is a
scribe with extra steps.

The method is a reasoned precaution and has not been evaluated in a trial. The
rationale comes from adjacent evidence on automation bias and skill decay, not
from a study of AI scribes and clinical reasoning, because that study does not
exist yet.

Any guide you build is yours. I have not reviewed it, which is why every
generated guide carries a signature field.

## Credit

The underlying practice, continuing to narrate after the patient leaves,
originates with **Dr Michelle Adams of Time to Grow Clinic**. The paper
formalises it as *speak before the reveal*, and this repository extends it to
other specialties.

Thank you also to **Dr Rob Selzer** for his input in developing the original
paper.

## Citing this

[![DOI](https://zenodo.org/badge/1352303121.svg)](https://doi.org/10.5281/zenodo.22331969)

The method:

> Jurblum M. *Speak Before the Reveal: Seven Solutions to Governing AI Scribe
> Deskilling Risk in Psychiatry and Mental Health Services.* Preprint,
> 28 July 2026. https://doi.org/10.2139/ssrn.7317778

The psychiatry guide: https://doi.org/10.5281/zenodo.22342673

This repository:

> Jurblum M. *Speak Before the Reveal: Reference Guide Skill.* Zenodo.
> https://doi.org/10.5281/zenodo.22331969

## Licence and disclaimer

[CC BY 4.0](LICENSE). Use it, adapt it, build on it, keep the attribution.

Read [DISCLAIMER.md](DISCLAIMER.md) before you use any of this. In short: this
is an aid to documentation practice and not clinical advice, any guide you
generate is your own clinical work and has not been reviewed by me, all AI
output must be reviewed by the person who generated it, and maintaining your own
templates and meeting your own documentation requirements remains yours.
