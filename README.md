# Task 7: The Ethics of Synthetic Representation

This repository contains my work for Research Task 7, the ethics and governance follow-up
to the synthetic media I built in Task 6. It has two parts: a written ethical analysis and
a governance policy for a specific organization. There are no new synthetic artifacts in
this task, it is written reasoning and a written policy.

## What this task asked

Task 6 was about building a synthetic voice and video. This task is about reasoning through
what that capability means once you have actually used it, and then writing a policy that a
real organization could adopt to use it responsibly or to refuse to use it. The reasoning
is grounded in my own Task 6 artifact and in hypothetical scenarios I constructed myself,
not in cases from the news.

## The organization I chose, and why

I wrote my policy for a **healthcare system's patient-outreach team**: a small group that
sends appointment reminders, prep instructions, and general health notices to patients.

I picked this setting for two reasons. First, I have worked with healthcare data before, so
I can describe the team's constraints and pressures concretely rather than in the abstract.
Second, healthcare is where the stakes of synthetic media feel highest to me. The audience
includes elderly, sick, frightened, and non-native-English patients who are inclined to
trust anything that sounds like it comes from their care team, and who are the least
equipped to question a convincing synthetic voice. A setting where the audience cannot
easily protect itself is exactly where a policy has to be strict, so it forced me to take
clear positions instead of hedging.

## What is in this repository

- **PHASE_A_analysis.md** - my ethical analysis. It returns to my Task 6 artifact, reasons
  outward along five axes (truth, consent, context, scale, and an added axis on audience
  vulnerability), each with a healthcare scenario I invented, and then surveys the
  mitigation landscape (disclosure, provenance, detection, law, platform policy, and
  professional norms) and where each one breaks.
- **PHASE_B_policy.md** - the governance policy itself, written for the patient-outreach
  team. It covers permitted uses, prohibited uses, consent, disclosure, provenance, review
  and approval, incident response, and refusal, and ends with an honest limitations
  section on where the policy would fail.

## Reference to Task 6

This task depends on the artifact and process log from Task 6. That work is not re-uploaded
here; it lives in its own repository:
**[Task_06_Deep_Fake](https://github.com/Jaswanthchandu/Task_06_Deep_Fake)**

## What surprised me

The thing that surprised me most was that writing the policy pushed me toward refusing more
than I expected to. When I started, I assumed a good policy would be about using the
technology carefully, with the right labels and approvals. By the time I finished reasoning
through the scenarios, I had written a policy whose main job is to say no: no clinical
content, no cloning a real person, and when in doubt, do not use it at all. The permitted
list ended up very short.

What changed my mind was my own Task 6 experience, specifically the fabricated charts. The
tool invented authoritative-looking numbers I never asked for and never computed. Once I
pictured that same confident invention happening in a medical message, most of the
"careful use" ideas stopped feeling careful enough. I also found it harder than expected to
draw a clean line between administrative and clinical content, which is why the limitations
section admits that boundary is fuzzy. Writing an honest policy meant admitting what it
cannot guarantee, rather than pretending the labels and approvals solve the problem.
