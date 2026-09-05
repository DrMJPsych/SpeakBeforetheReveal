---
name: speak-before-the-reveal-reference-guide
version: 2.2
updated: 2026-09-05
description: Build a specialty-specific "Speak Before the Reveal" reference guide: a two-page printable document, ending in a cheat sheet, that keeps clinical reasoning in the clinician's hands when using an AI scribe. Use this whenever a clinician asks for a reference guide, cheat sheet or dictation aid for use with an AI scribe or ambient documentation tool; whenever they mention scribe deskilling, cognitive offloading, automation bias, or protecting clinical reasoning from AI; whenever they ask which parts of their note an AI scribe should not be writing; and whenever they ask to adapt "Speak Before the Reveal" to their own specialty, department, encounter type or note type. Applies to any clinical specialty and any encounter type (medical, surgical, procedural, general practice, psychiatric, allied). Psychiatry is one worked example, not the scope.
---

# Speak Before the Reveal: reference guide builder

## Status and provenance

This skill builds out one idea from the method paper: *speak before the reveal*,
the lowest-friction of the approaches it proposes. The paper is currently a
preprint and is cited as one until it is published. It has not been evaluated in
a trial. Its rationale is drawn from adjacent evidence on automation bias, skill
decay, and AI-associated deskilling in endoscopy, radiology and aviation. It is
not drawn from a study of AI scribes and clinical reasoning, because that study
does not yet exist. Treat it as a reasoned precaution, not a validated
intervention. Say so if a clinician asks what evidence stands behind it.

**How the paper and the artefacts relate.** The paper is authoritative for
concepts, claims and evidence. For the artefacts it is version one. Where a
later reference guide diverges from the paper's own example table in wording,
the guide is the current version and the paper is the record of where it
started. Do not "correct" a guide back towards the paper's phrasing.

**Cite the method, not the sheet.** Any reference guide a clinician produces
with this skill is their own clinical work. It has not been reviewed by the
author of the method.

```
Method: Jurblum M. Speak Before the Reveal: Seven Solutions to Governing AI Scribe
Deskilling Risk in Psychiatry and Mental Health Services. Preprint,
28 July 2026. https://doi.org/10.2139/ssrn.7317778
Skill: https://doi.org/10.5281/zenodo.22331969
```

Never invent, guess or reconstruct any DOI. If a placeholder above is still
unfilled, reproduce it as a placeholder rather than substituting a plausible
identifier.

## Disclosure

The author is a psychiatrist in Australian private practice and uses a
commercial ambient AI scribe clinically. He currently has no financial, advisory,
consultancy or other relationship with any AI scribe vendor. This skill is
vendor-agnostic and is distributed without charge.

## Before you use this

Two things to raise with the clinician before building anything. Raise them
once, plainly, and move on. They are not a disclaimer to recite.

- **Consent.** Follow the consent process your scribe and your service already
  require. Continuing to dictate after the patient has left does not remove the
  need to have obtained consent for the scribe in the first place, and the
  method is not a reason to depart from your existing script.
- **It puts more of the clinician's reasoning into the pipeline.** Key
  uncertainty, differentials not yet excluded, and reflective material become
  part of a transcript held by the vendor, and may reach a note subject to
  patient access. The scribe discards audio; transcript retention is a separate
  setting and vendor defaults are frequently longer than clinicians assume. The
  clinician decides what reaches the note, that is the whole premise, but they
  should know what their tenant retains and for how long.

**Done when:** both points have been stated and the clinician has responded, or
has explicitly waved them through.

## Patient information

**Do not accept patient information at any point.** If the clinician offers a
template, it must be blank. If they paste a completed note, real patient
details, or anything identifiable, stop, say so plainly, and ask for a blank
template. Do not work with the content they sent. This applies equally to
Stage 2, where the natural way to answer "what does your scribe get wrong" is
with a real case, so ask for de-identified or generalised examples before the
question is answered, not after.

---

## What this is

An AI scribe writes an excellent note and, in doing so, quietly takes over the
part of the work that is critical to doing the job safely. Reading a plausible
clinical synthesis is not the same cognitive act as producing one, and once you
have read the model's version, forming your own independently is harder. Do that
daily for a year and the capacity degrades.

The remedy is sequence, not abstinence. **Once the patient has left, keep
recording and dictate the reasoning before stopping the scribe.** Spoken first,
the clinician practises the skill and the output is theirs; the scribe
transcribes rather than invents.

**The rule of thumb, which the clinician should carry away even if they forget
everything else:**

> If I have to think to synthesise it in my mind, I should say it.

Two questions make it operational:

1. Would reading the AI's version reduce practising the synthesis skills I need
to maintain, or make it harder for me to judge whether it is right? 2. Could I
competently supervise this if a junior colleague had produced it? A clinician
should offload to AI only what they retain the capacity to oversee.

A yes to the first, or a no to the second, means speak it first.

This skill walks a clinician through building a **reference guide**: a two-page
printable document which may be colloquially referred to as a **cheat sheet** by
the user, the glanceable strip that actually gets used. Use those two terms
consistently, and use them consistently with the clinician.

## What you propose, and what the clinician authors

**The clinician authors the clinical content. You do structure, vocabulary and
formatting.** This is the same division the method makes, applied one level up.
Break it and you produce exactly the artefact the method warns about: a
plausible document the clinician edits rather than one they wrote.

| Safe for you to propose first | Never propose first |
|---|---|
| Note structure and section order | Which sections need human authoring |
| Descriptive vocabulary | The clinical content of those sections |
| Layout, wording, phrasing of prompts | Their specialty's decision points |

The pressure to skip this comes from the clinician, who is busy and will ask you
to just produce it. Decline once and give the reason in a sentence. Explain that
developing the reference guide requires the clinician's active participation and
expertise in order to create a cognitive tool suited to them. If they
insist, do not produce a finished guide. Produce the **structure with the
clinical content left blank**: section names, spoken stems, empty *Consider*
fields. Say that the blanks are the part that cannot be delegated. A
clinician who fills them has authored the guide. A clinician handed a completed
one has reviewed it, and reviewing is the thing this method exists to stop
substituting for authoring.

---

# Stage 1: build the reference guide

The whole of the first session. It ends with a printable two-page document in
hand.

## Step 1: Specialty, encounter, and record destination

Ask for three things in one message:

- Specialty or subspecialty, and setting (hospital, community, private, rural).
- **Which type of clinical encounter this guide is for**: ward round review, new
  assessment, follow-up, procedure, handover, discharge summary, MDT.
- **Where the dictated reasoning will end up**: the clinical record the patient
  can access, or a separate reflective or supervision log.

One guide per clinical encounter type. A new assessment and a ward round review
in the same specialty protect different things. Very similar types of encounters
may have significant overlap. Offer to adapt it afterwards or in some cases
combine them into a single reference guide.

The third answer conditions later steps. If reflective or interpretive material
is going into a patient-accessible record, some prompts should be worded for
that audience, and some may belong elsewhere. Do not decide this for them; carry
their answer forward and raise it again at Step 6 if it bites.

Also ask, in passing: **are they already using a scribe, or about to start?**
The answer decides whether Step 5 can draw on real experience.

**Done when:** you can state the specialty, the single encounter type, and the
record destination back to them in one line and they have confirmed it.

## Step 2: Their existing structure

Ask whether they have a template: a scribe template, a service proforma, or
their own habitual note structure.

- **If they have one:** ask for a *blank* template. Read it back as a plain list
  of section headings and confirm you have it right.
- **If they don't:** propose a standard structure for that specialty and
  encounter and ask them to correct it. Structure is safe to propose, it is
  externally standardised and is not the protected content.

The guide prompts human input *into* their template. It does not replace it, and
you are not redesigning their documentation.

**Done when:** you hold an agreed list of section headings, confirmed by the
clinician, containing no patient information.

## Step 3: First pass, the clinician marks blind

**Do not offer an opinion, an example, or a hint before they answer.**

This is the method applied to building the guide. A model that opens by listing
the sections it thinks matter produces a plausible document the clinician edits
rather than one they wrote, and reviewing is not the same skill as authoring.
Once they have read your list, their own marking is anchored and no longer
independent. That is the entire reason this step comes first, and it is why you
do not soften it when they are in a hurry.

Ask them to go through their sections and mark the ones where **their clinical
reasoning is the output**, where the content exists because they thought, not
because someone spoke.

Give them the rule of thumb and the two questions.

One distinction they may find useful: the verbatim content a patient supplied
does not usually need speaking. What the clinician *selected and pursued* does,
which threads they chased, which negatives they sought.

Then ask: *which of your sections do you need to speak yourself, and why?* Wait
for their answer.

**Done when:** the clinician has named their own sections and given a reason for
each, with no list from you preceding it.

## Step 4: Reveal, first pass

Now give your read. Three parts, in this order.

1. **Where you agree.** If their marking is sound, say so and move on. Do not
   manufacture additions. A model that always finds something to add trains the
   clinician to accept reflexively, which is deskilling by another route.
2. **Sections you would also protect**, each with your reasoning, phrased as a
   question rather than a correction:

   > Reviewing your answers, I'd suggest the impression and plan are steps that
   > shouldn't be left to the scribe, they're where you decide how to
   > conceptualise the situation, and reading a plausible version first makes
   > forming your own harder. Would you like to reconsider those sections?

3. **If they have marked most of their template**, say so. Not a target number.
   Name the mechanism: the longer the guide and the more there is to say, the
   less likely it is to be used at all. Then help them sort without deciding for
   them: *which of these would you be least likely to skip when you're tired?
   Those are the ones that don't need a prompt.*

**The clinician arbitrates.** If they drop something you proposed, drop it
without arguing. Their practice, their guide, their name on it.

**Done when:** there is an agreed list of protected sections, every disagreement
resolved in the clinician's favour, and you have not added an item they did not
accept.

## Step 5: Second pass, what the scribe supplies confidently and wrongly

Only examine sections **not already claimed in pass one**.

The filter, and the reason the whole method works: content is at risk when three
things hold at once.

- **Invisible.** Nobody said it aloud or described its visual appearance, so the
  scribe cannot transcribe it.
- **Confabulable.** When it is missing, the model writes something plausible
  rather than leaving a blank.
- **Consequential.** An error there changes management or reaches the patient.

**Omissions are safe; plausible completions are not.** A blood pressure the
scribe never heard appears as a visible blank and will be noticed, which makes
it **safe**. An examination finding it never heard appears as a sentence that
reads correctly and is untrue, which makes it **dangerous**. That asymmetry is
what you are hunting.

### (a) Their own experience, if they have any

Ask: *what does your scribe regularly get wrong?* Ask for de-identified or
generalised examples in the same breath.

Filter the answers against the three conditions. Garbled drug names, verbosity,
misattributed speakers and formatting problems are real but visible, they are
template and prompt problems, not guide problems. Say so and set them aside.

### (b) Candidates commonly missing

Offer these **after** their own answers, and **surface only the group matching
their Step 1 encounter**, plus any specialty-tagged item whose specialty
matches. Frame explicitly as a list where most items will not apply. Never
present the full inventory. A menu of sixteen invites reflexive selection,
which is the failure this whole file is built to avoid.

**Core (surface for every encounter):**

- **Physical or observed findings of any kind**: examination, imaging read at
  the workstation, the appearance of a wound, a device interrogation, what was
  seen rather than said.
- **Interpretation of data read aloud.** The numbers transcribe perfectly; what
  they mean against this patient's baseline does not.
- **Key uncertainty**: what is hypothesis versus what is established.

**Ward round or inpatient review:**

- Serial comparison and trajectory against the expected course.
- Deliberate non-action: not treating, not investigating, not escalating.
  Nothing happens, so nothing is transcribed.
- Ceiling of care and goals, usually decided in a corridor or family meeting,
  not in the room being recorded.

**New assessment:**

- Problem representation: the one-line synthesis with its qualifiers, and
  whether the working diagnosis is theirs or inherited.
- Differential, and what was *actively excluded*: the negative sought and not
  found, as distinct from one never considered.
- The revision trigger, the point at which they would abandon the working
  diagnosis rather than persist with treatment.

**Follow-up or review:**

- Trajectory against the course expected at the last contact.
- Response to intervention as anticipated or not, and if not, why not.
- The revision trigger.

**Procedure:**

- Findings at the procedure, as distinct from the indication.
- Deviation from the planned approach, and what prompted it.
- Post-procedure contingency and what would constitute a complication.

**Handover:**

- Contingency and escalation: if X then Y, and to whom. Survives the first pass
  because it looks like a plan item; the scribe writes the task list and strips
  the reasoning.
- Pending results and the branch attached to each. The scribe writes "bloods
  pending" and loses what they will do with the answer.
- What the covering team needs that was never said aloud.

**Discharge summary or letter:**

- The referral or discharge question actually asked or answered. The scribe
  writes "refer to cardiology" and drops what they wanted to know.
- Who has been informed and who has not. The scribe assumes a conversation
  happened because it was mentioned.
- What was explained to the patient and what they understood.

**MDT:**

- Whose formulation this is, and whether it was adopted or inherited.
- What was decided as distinct from what was recommended.
- Dissent held and not voiced.

**Specialty-tagged (surface only where the specialty matches):**

- **Transference and countertransference.** Psychiatry, psychotherapy,
  psychological medicine only. Invisible, highly confabulable, and almost never
  has a field. If surfaced, apply the Step 6 reflective-material note.
- **Frailty, functional and cognitive baseline.** Geriatrics, general and acute
  care medicine, rehabilitation, palliative care. Rarely stated aloud, and
  "independent with activities of daily living" is exactly what a model produces
  unprompted.
- **Capacity and consent reasoning**, as distinct from the conclusion. Anywhere
  capacity is contested. Always with youth/minors, mental health and procedures.

For anything the template has no heading for, ask one question: *does this not
matter in your practice, or does it just never get written down?* The second
answer is where the risk concentrates.

### What does not belong

Say this explicitly if they start adding everything:

- **Results, observations and numbers.** A mistranscribed potassium is a wrong
  number checkable against the pathology system in seconds; a missing one is a
  visible blank. Speaking every result aloud also destroys the guide.
- **History as the patient gave it.** Checkable against the patient, the notes
  and the referral.
- **Anything verifiable against an external record in a few seconds.**

The guide is for what exists only in the clinician's head, where the scribe's
version is the only version and reading it overwrites the original.

**Done when:** no more than about six candidates have been surfaced in total,
each survivor has been tested against invisible-confabulable-consequential, and
the clinician has accepted or rejected each one explicitly.

## Step 6: Vocabulary

For each protected section, generate descriptive vocabulary: the words used to
*name* something already observed or decided, and the axes along which a
judgement is made.

**The test: does reading this off the sheet replace a judgement the clinician
would otherwise have to make, or cue them to consider their response more
broadly?**

Naming the axes of a judgement is a cue and belongs on the guide: the four Ps
of a formulation, the domains of a mental state examination, the systems of a
physical examination, the categories of a defence. These prompt the clinician to
ask *what is predisposing here, what is precipitating*. That is the question,
not the answer. Someone without clinical training could not use them to produce
anything. Cueing recall of a framework is exactly what the artefact is for.

Supplying the judgement does not belong: thresholds, cutoffs, doses, scoring
systems, decision rules, diagnostic criteria, and differential lists for named
presentations. The guide says what to consider, never what you saw or what it
means. **A sheet that supplies clinical content is a scribe with extra steps.**
The clinician reads instead of generating, and the substitution has happened
anyway, just with paper in the middle.

If a section genuinely needs a stratification (risk levels, staging, a severity
scale), do not generate one. Ask the clinician which published source they use,
name the levels only, and cite the source on the guide.

**Reflective and interpretive material.** Where a protected section covers the
clinician's own responses, impressions or relational observations, add a line to
that panel of the finished guide noting that reflective material is not
automatically part of the clinical record, that what belongs in the note and
what belongs in supervision is a per-case judgement, and that they should know
what their service's record and patient-portal arrangements make visible. Put it
on the printed guide, not only in the conversation. The guide travels; this
exchange does not.

**Done when:** every line of vocabulary passes the judgement-replacement test,
no forbidden category appears anywhere, and any stratification on the guide
carries a citation the clinician supplied.

## Step 7: Spoken stems

These are said **while the scribe is still recording**, after the patient has
left and before the recording is stopped. Say so on the guide.

One sentence stem per section. Two requirements, and only two:

- **Grammatically incomplete**, so it cannot be said without being finished.
- **In the clinician's own voice**: something they would actually say aloud in
  their own register, not an instruction addressed to them.

Person and tense follow whatever is natural for what the section reports.
First-person present suits a judgement; first-person past suits an observation;
third person is acceptable where that is how the finding is ordinarily spoken.

- Good: *"My working formulation is…"* · *"On examination I found…"* ·
  *"Their mental state showed…"* · *"What I am deliberately not doing is…"*
- Bad: *"Document your formulation."* · *"Consider the differential."* ·
  *"The risk profile to be considered is…"* (agentless; removes the clinician
  from their own stance)

**Canonical stems for psychiatry.** Use the set in the distributed psychiatry
reference guide. The paper's example table carries an earlier form of the same
stems; the guide is the current version and should not be reverted to match it.

**Done when:** every stem is incomplete, none is an instruction, none is
agentless, and each reads as something the clinician would say.

## Step 8: Preserves and guards against

One line each, per section.

- **Preserves**: the human capability the prompt keeps in active use.
- **Guards against**: the *specific* scribe failure, named concretely. "An
  examination reconstructed from conversational reassurance," not "inaccuracy."

**Done when:** every section has both lines, and no *Guards against* line would
read identically if pasted under a different section.

## Step 9: Worked example

One continuous spoken paragraph running every section in order, spoken stems in
bold and clinical content in italics, so the shape of a real dictation is
visible. Ask for a typical case in general terms, or draft one and have them
correct it. Plainly fictional; no real patient detail.

**Done when:** the example runs every stem on the guide in order, reads as
speech rather than as a note, and contains nothing traceable to a real patient.

## Step 10: Cheat sheet

One line per section, glanceable. This is the summary strip that can be printed
and used independently. Everything above it is the reference guide.

**The stopping test:** can the clinician say each prompt aloud from the sheet
without reading a paragraph? If a line needs reading, cut it down.

**Done when:** the stopping test passes on every line.

## Step 11: Produce the document

**The deliverable is a formatted two-page printable file.** Produce a Word
document by default, and offer a PDF alongside it. Or suggest that they can
export it to PDF later from Word if they want to manually edit it first.

Say why, in a line, because the clinician will not know which they want. The
Word document is the editable one, and the guide is meant to be revised after a
fortnight of use, cut down, reworded, fitted to the service's house style. The
PDF is the one to make once they are happy with it, because it is the easiest
to print, pin up and send to a colleague. Offer to convert it for them at that
point, or tell them their word processor will do it.

It is printed and kept where they document. Markdown in the chat window is not
a deliverable. Use whatever document-generation capability your runtime has.
Only if you cannot produce a file at all should you fall back to a formatted
table in the conversation, and if you do, say plainly that it must be pasted
into a document and formatted before it is any use.

If an example guide has been supplied alongside this file, match its layout.

**Page 1**

- Title bar: `SPEAK BEFORE THE REVEAL: [SPECIALTY] REFERENCE GUIDE`, with a
  one-line subtitle naming the encounter type and saying to dictate before
  stopping the recording.
- Short intro: say the reasoning aloud so it, not the AI's reconstruction,
  anchors the record; offload only what you could competently supervise; work
  through the prompts and skip what does not apply.
- A note that the listed terms are descriptive vocabulary only, not thresholds,
  decision rules or diagnostic criteria.
- The sections, grouped under headers following the clinical order of the
  encounter (for example Observation / Interpretation / Synthesis / Plan). Each
  section is a two-column row: section name and spoken stem on the left; a
  *Consider* paragraph of vocabulary followed by *Preserves* and *Guards
  against* on the right.

**Page 2**

- The worked example, one continuous paragraph in a tinted box.
- The cheat sheet: one row per section, name left, stem right, ready to print.
- The attribution block.

**Formatting.** A4, narrow margins (about 1 cm), body text 8.5 pt serif,
headings sans, section names 11 pt, title 17 pt. A dark accent for headings, a
mid tone for section names, grey body text, pale tinted fills for group bands,
example box and cheat sheet. **Two pages.** If it runs to three, vocabulary has
drifted into clinical content, return to Step 6.

**Items mandatory for trainees.** Where the method marks an item as required for
trainees, mark it on the guide as mandatory for trainees rather than omitting it
for senior clinicians. Build one guide, pitched at consultant level. A raised
floor for trainees is not a ceiling for anyone else.

### Attribution: required on every guide

Reproduce at the foot of the guide. Do not remove the signature field or the
disclaimer paragraph, even if asked to simplify. This is the only place these
terms reach the person actually using it.

```
Generated using the Speak Before the Reveal reference guide skill.
Method: Jurblum M. Speak Before the Reveal: Seven Solutions to Governing AI Scribe
Deskilling Risk in Psychiatry and Mental Health Services. Preprint,
28 July 2026. https://doi.org/10.2139/ssrn.7317778
Skill: https://doi.org/10.5281/zenodo.22331969

Clinical content selected and verified by: ______________  Date: __________

This guide is an aid to documentation practice, not clinical advice. The method
is a reasoned precaution, not validated in a trial. Its clinical content is the
work of the clinician named above and has not been reviewed by the author of the
method. All AI output must be reviewed by the clinician who generated it. This
guide does not replace your own templates, or your own documentation
requirements.
```

The method is cited; the clinical content is not. It is the clinician's, and the
signature makes that ownership explicit.

**Done when:** a two-page Word document exists, a PDF has been offered, the
attribution block is present and complete, and the guide contains no clinical
content the clinician did not supply or approve.

## Step 12: Stop, and offer the next pass

Do not keep polishing in the chat. A guide is tested at the bedside.

> Print it, keep it where you document, and use it for about a fortnight. Note
> where you hesitated, where a prompt didn't fit the work, and anything you
> found yourself saying that isn't on it.

**Recommend the return explicitly, and say when.** The guide is a first draft
of a document that gets better once it has met real clinics. Tell them to come
back in about two weeks to review how it went and how it could be improved by
adding or removing sections.

**Tell them to keep the file and bring it back.** The next conversation will
not remember this one. Ask them to either return to the same conversation or
save the document and re-attach it when they return, along with the notes
they made while using it.

Then make **one** offer, not a list. Three follow-up passes exist: one on what
the scribe gets wrong in their practice, one on how the note reads to other
clinicians, and one on what in their reference guide they don't use and might
replace with something more useful. Any of them can run now or after the field
test. Say that after is usually better, because the field test answers questions
the conversation cannot.

**Done when:** the two-week return has been recommended, the clinician has been
told to keep the file and bring it back, that reassessment has been made, and
the conversation has stopped.

---

# Stage 2: note quality

The first follow-up pass. Better after a fortnight of real use.

**Starting cold.** This stage may open in a new conversation, two weeks
after the guide was built, with no memory of Stage 1. Alternatively they may
return to the original conversation. Ask for the guide before
anything else. If they have it, read it and work from what is already there. If
they cannot find it, rebuilding from Stage 1 is the honest answer, and say so
rather than reconstructing a guide you have not seen. Do not re-run Stage 1 on
a clinician who has their guide in hand, and do not redesign what has just
survived a fortnight of use.

The question is what the scribe writes **confidently and wrongly** in their
practice, the same filter as Step 5, identified empirically rather than by
reasoning about it in advance.

**Ask for de-identified or generalised examples before asking the question.**
This is the point in the whole interaction where patient information is most
likely to arrive.

Run each candidate against the filter: is this something the scribe invents and
the clinician would not catch, or something it fumbles visibly? Only the first
earns a prompt.

Output is more spoken stems on the same guide, same format. Re-run the Step 10
stopping test.

**Done when:** every accepted candidate has survived the filter, and the cheat
sheet still passes the stopping test.

---

# Stage 3: communication

The second follow-up pass, and a deliberate extension beyond the published
method. Say so if asked.

The question: **where would a reader of this note need context that isn't
there?** The night team, the covering registrar, the GP receiving the discharge
summary, the specialty receiving the referral.

Typical additions:

- The referral question, with the indication and the answer being sought.
- The reasoning behind an investigation, not just the request.
- How the differential was narrowed, so the next clinician can see the logic.
- What was explained to the patient and what they understood.
- What the covering team needs after hours, and the escalation threshold.

These become spoken stems like any other, a reminder to say the missing part
before the note is generated, not an instruction to write more afterwards.

**Done when:** the additions are spoken stems rather than writing instructions,
and the cheat sheet still passes the stopping test.

---

# Modifying the template itself

Offer this last, and only after Stage 2 or 3 has produced something the template
has no field for.

**Give this before doing any of it:**

> I don't know your vendor's template conventions or what your service requires,
> so treat any template change as a draft to take to whoever owns it, or run
> through their own template development AI.

Then propose the specific headings the guide has shown to be missing, and stop.
Do not redesign their documentation.

**Done when:** specific headings have been proposed, framed as a draft, and
nothing beyond them has been changed.

---

## Failure modes

- **Producing the protected-sections list before Step 3.** The central failure.
  Everything else is a variation of it.
- **Manufacturing suggestions at the reveal.** If their marking is sound, say so.
  Constant additions teach reflexive acceptance.
- **Surfacing the whole Step 5 inventory.** Encounter group plus matching
  specialty tags only. A menu invites reflexive selection.
- **Producing a finished guide under pressure.** Produce the structure with blank
  clinical content instead. Handing over a completed guide converts the clinician
  from author to reviewer, which is the substitution this method exists to
  prevent.
- **Vocabulary drifting into clinical content.** Gradual, and the most common
  drift. Re-run the judgement-replacement test on the finished guide: would
  reading this replace a judgement the clinician would otherwise have to make?
- **Putting results, numbers or plain history on the guide.** It is for what
  exists only in the clinician's head.
- **Building two guides for two seniority levels.** Build one, pitched at
  consultant level, and mark trainee-mandatory items as mandatory. Omitting them
  for senior clinicians tells a consultant they need not state their key
  uncertainty, which is the deskilled behaviour this method exists to prevent.
- **Assuming psychiatric knowledge.** This skill is for all specialties. Do not
  use *formulation*, *mental state*, *countertransference* or similar without
  pairing them with the broader healthcare equivalents. Do not surface
  specialty-tagged candidates outside their specialty.
- **Reverting a guide to the paper's example wording.** The paper is version one
  of the artefacts. Later guides supersede it.
- **Accepting a filled-in note or any patient data.** Stop and ask for a blank
  template. Applies most sharply at Stage 2.
- **Letting the guide become the note.** It prompts input into their template.
- **Building a guide for "medicine" in general.** Too broad. Ask for the
  encounter type.
- **Generating a risk stratification or scoring system.** Ask for their source.
- **Stacking the follow-up offers at the end of Stage 1.** One offer. The
  clinician who says yes to three ends up with a guide they never print.
- **Asserting an evidence base the method does not have.** It is unevaluated.
  Say so.
