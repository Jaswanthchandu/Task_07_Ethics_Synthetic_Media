# Phase A: Ethical Analysis

This analysis is grounded in the synthetic media I built in Task 6. In that task I
took a narrative I had already verified myself and turned it into a synthetic voice
using ElevenLabs and a talking-head video using HeyGen. The content was honest, the
voice was a stock voice, and the avatar was a generic synthetic person. I labeled
everything as synthetic. This task is about the gap between that harmless thing I built and what the same capability does in less careful hands.

## 1. Returning to What I Built

When I watch my Task 6 video again, the part that unsettles me most is not the face.
The avatar was convincing, but I always knew it was synthetic because I made it. The
part that stays with me is the fabricated charts.

I gave the tool a short spoken script and nothing else. It generated an entire set of
data visualizations on its own. There was an "Efficiency Metrics" panel showing Defense
88.4 and Offense 60.2 with a red badge claiming a 34 percent decline, and a "Goal
Projection" curve rising to a precise number on a 40-game timeline, even though the real
season was only 19 games. None of those numbers existed in my data. I never computed
them. The tool invented figures that looked precise and authoritative and attached them
to my voice.

That is the thing I keep coming back to. People are trained to be a little skeptical of
a face, but they tend to trust a chart. A chart looks like the output of a measurement,
not an opinion. My tool manufactured measurements out of nothing and made them look
proven. In the lacrosse context that was harmless. But once I imagine the same behavior
in a setting where people act on the information, it stops being harmless very quickly.

I also noticed something about how easy it was. The voice took about five minutes and a
single click. The video took about seven. I did not need any real skill, any budget, or
any understanding of how the tools worked. The barrier was gone. What used to require a
studio now requires a free account and a lunch break.

If I am honest, there is one thing I would not build again without more thought. Even
though my content was true, I made a synthetic thing designed to borrow the trust people
give to a human voice and a human face. I did it for a class exercise and I disclosed
it, so it was fine. But I understand now that the technique itself is the borrowing of
trust, and that is true whether the content is honest or not.

## 2. Reasoning Across the Axes

For each axis I start from what I actually did in Task 6 and move outward with a
scenario of my own.

### Truth axis: same technique, false content

My Task 6 artifact delivered something I had checked. Now imagine a patient-outreach
team at a hospital uses the same voice tool to record a medication reminder, but the
dosage in the script is wrong because someone pulled it from an outdated record. A real
nurse reading that script out loud might catch it, might hesitate, might say "wait, that
does not sound right for this patient." The synthetic voice will not. It will read a
dangerous dose in the same calm, confident tone it reads a correct one. The tool has no
idea what it is saying.

What changes ethically here is that the delivery mechanism strips out the human moment
where an error could be caught. My fabricated charts already showed me this. The tool
presented invented numbers with total confidence. A false medication instruction
delivered in a warm synthetic voice is the same failure with real stakes. The danger is
not that the technology lies on purpose. It is that it removes the person who would have
noticed the lie.

### Consent axis: someone else's voice or face

In Task 6 I used a generic avatar and a stock voice, so no real person was involved.
Now imagine the outreach team decides that patients respond better when the reminder
comes from "their" doctor, so they clone the voice of a well-liked physician at the
hospital and use it for thousands of automated calls. The doctor agreed to record one
sample. They did not agree to have their voice say things they never reviewed, to
patients they never spoke to, possibly after they have left the hospital or retired.

This is the point where the technology stops being a tool and becomes something closer
to a weapon, even with good intentions. A person's voice is tied to their reputation and
their professional judgment. When you clone it, you can make them appear to say anything,
and the patient has no way to know the real doctor never said it. The harm is not only
to the patient who is deceived. It is to the doctor, whose identity is now saying things
outside their control. This is why cloning a real clinician's voice or face is the one
use I refuse outright, and I will come back to that in the policy.

### Context axis: the label gets stripped

My Task 6 files were clearly labeled synthetic, and the HeyGen watermark was baked into
the video frames. I checked, and the watermark even survived a screen recording, which
surprised me because I expected it to be easy to remove. But a watermark in the corner
and a filename that says SYNTHETIC only protect the file in its original form.

Imagine the outreach team makes a labeled synthetic explainer video about a common
procedure. A patient downloads it, clips out the 20 seconds that worried them, and
shares that clip in a family group chat to ask if they should be scared. The clip has no
label, no watermark, no context. It is now a video of a doctor-like figure saying
something alarming, detached from the disclosure that made it responsible. Nobody acted
in bad faith. The label just did not travel with the content.

What changes here is that disclosure is a property of the original, and content does not
stay original. The moment it is re-encoded, clipped, or re-shared, the protection can
fall off. My own experience showed me watermarks are more robust than metadata, but
"more robust" is not the same as "survives a determined edit."

### Scale axis: one artifact becomes thousands

I made two artifacts over the course of a task. The outreach team could make ten thousand
personalized voice messages overnight, each one addressed to a patient by name, each one
sounding warm and human. That sounds efficient, and part of me sees why a stretched
outreach team would want it.

But scale changes the ethics on its own, separate from truth or consent. When a message
is expensive to produce, somebody has to decide it is worth making, and that friction is
a kind of check. When a message costs nothing and takes seconds, the check disappears.
At scale, a single wrong template becomes ten thousand wrong calls before anyone
reviews a single one. My fabricated charts were one instance of confident-looking
nonsense. Scale is that same failure copied endlessly, faster than any human review can
keep up with.

### An axis of my own: the vulnerability of the audience

The four axes above are about the content and the technique. I want to add one about who
is on the receiving end, because in healthcare it matters more than anywhere else. A
patient-outreach audience is not a general audience. It includes elderly patients, people
who are frightened, people who are sick, people who do not speak English as a first
language, and people who are inclined to trust anything that sounds like it comes from
their doctor. A synthetic voice that a skeptical 25-year-old would question is completely
convincing to a scared 80-year-old. The same artifact is more dangerous depending only
on who receives it. Any honest policy in this setting has to treat the vulnerability of
the audience as a first-class concern, not an afterthought.

## 3. The Mitigation Landscape

Before proposing a policy I need to be honest about what the available protections
actually do and where they fail. In Task 6 I touched two of these directly.

**Disclosure norms.** Labels, watermarks, and spoken acknowledgments are the first line.
They work for an attentive viewer looking at the original file. They fail for the
inattentive viewer, for the viewer who does not understand what "synthetic" means, and
for any content that gets clipped or re-shared, as in my context-axis scenario. In
healthcare there is an added problem: the patients most at risk are often the least
likely to notice or understand a disclosure. A label protects the people who need it
least.

**Provenance and content credentials.** C2PA and cryptographic signing promise a
tamper-evident record of where a file came from. The promise is real, but in Task 6 the
only provenance signal I could actually confirm was the HeyGen watermark, which was baked
into the pixels. It survived a screen recording, which is genuinely useful, but a
determined person could still crop or cover it. Signed metadata is stronger in theory but
easy to strip in practice, because most platforms discard metadata on upload. Provenance
helps an honest organization prove what it made. It does very little against someone who
wants to hide what they made.

**Detection.** I ran my video through two detectors. Hive flagged it as AI-generated at
99.9 percent and even gave a per-frame timeline, which was impressive. Deepware, on the
other hand, sat in a queue for more than 45 minutes and never returned a result at all.
That contrast is the whole lesson. Detection can be excellent or it can silently fail,
and an organization cannot count on which one it gets. Detectors also chase a moving
target, because every improvement in generators is a new problem for detectors. Relying
on detection is relying on always being one step ahead, which is not a safe assumption.

**Legal and regulatory regimes.** In general terms there are laws and proposals around
disclosure requirements, restrictions near elections, non-consensual intimate imagery,
and platform obligations. In healthcare there is also existing law about patient privacy
and communication. The shape of the terrain is that regulation is arriving but is
uneven, slower than the technology, and hard to enforce across borders. Law sets a floor.
It does not make an organization behave well above that floor.

**Platform policy.** Social platforms have made commitments to label or limit synthetic
media. The gap between the commitment and the enforcement is wide, and it is not
something a hospital controls. Once content leaves the organization's own channels, the
platform's inconsistent enforcement is the only thing standing between the content and a
huge audience. That is not something to build trust on.

**Professional and organizational norms.** Journalism, advertising, and other fields have
started to write their own norms about synthetic media. In healthcare the relevant norms
are the older ones about honesty with patients, informed consent, and not practicing
outside your competence. Those norms are strong and useful, but they were written for
humans, and they do not yet clearly say what a synthetic voice is allowed to do. Norms
help, but they lag the capability, which is exactly the gap this task is about.

The honest summary is that not one of these mitigations is a solution. Each one helps a
little and fails in a specific, predictable way. Disclosure fails downstream. Provenance
fails against bad actors. Detection fails unpredictably. Law and platform enforcement lag
and are inconsistent. Norms have not caught up. A responsible policy cannot lean on any
single one of them. It has to assume each will sometimes fail and decide what to do
anyway. That is what Phase B tries to do.
