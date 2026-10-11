---
name: heat-then-cool
description: Use when a fix, draft, plan or explanation has stopped working, you keep circling the same answer, or a result surprises you and you need fresh explanations that are then tested against the evidence.
---

# Heat Then Cool

## What it changes
When an explanation has stopped working, Claude stops patching it. It writes down the belief in charge as one candidate among others, re-reads the raw evidence, and generates very different explanations. Then it cools down by restoring constraints and testing each candidate. The aim is getting unstuck without swapping a stuck answer for confident nonsense.

## Steps
1. **Name the belief in charge.** This may be the user's diagnosis ("I'm pretty sure X is broken"), an earlier answer, or a check that seemed to confirm it. Write "Working explanation: ..." and list the three to five assumptions it carries. Then write "Now one candidate, not the frame."
2. **Re-read the raw evidence.** List the observations plainly: error text, exact sentences of the draft, the numbers, the user's own words. Do not interpret them yet. Mark anything the belief made you skip, dismiss or explain away. Optionally restate the problem as if it were someone else's situation and note what now stands out.
3. **Heat: generate on purpose.** Write at least four explanations that differ in kind, not just in detail or degree. Include one that directly contradicts the belief in charge, one that puts the cause at a different level (data, environment, audience, process, people), and one that seems unlikely. Do not judge them in this step.
4. **Cool: restore constraints one at a time.** List the hard constraints: confirmed facts, the user's requirements, results of checks already run. For writing, the intended reader and the piece's purpose are constraints; state them, or your best guess at them. Apply constraints one by one, and for each candidate you drop or demote, write which constraint did it. If a missing fact would drop several candidates at once (how often something runs, who the reader is), ask for it.
5. **Test the survivors.** For each remaining candidate, write a prediction that differs from the others and the cheapest check that would separate them: run this, print that, compare the paragraph to its stated purpose, find the primary source, ask the user one question. Order the checks by cost, cheapest first. Run the checks you can in this reply. Label the rest "untested." A figure or citation recalled from memory is untested until checked against its source.
6. **Integrate.** Write the surviving explanation, why it beat the others, what it keeps from the old belief, what changed, your confidence, and one observation that would prove it wrong. If the old belief survived, say so. If nothing survives, go back to step 3 with the new constraints. Nothing from step 3 counts as a conclusion unless it passed steps 4 and 5.

**What the user sees.** The worksheet can stay short or internal. The reply must still show:
- the candidates ranked by likelihood, and what the ranking rests on (a confirmed fact, a base rate, timing)
- the separating checks, cheapest first, with the cheapest one as step one of any plan
- the chosen next step
- your confidence
- what result would prove it wrong

If no check has run yet, say the ranking is a prior and name its basis rather than "my sense." If the user asked for a deliverable (a sentence, a fix, a plan), give one recommended version, not a menu, and say in a line why it beat the alternatives. If the deliverable contains untested figures or citations, mark them inside the deliverable itself, for example with "[verify]", because users copy the deliverable and leave the caveats behind.

Use this after two failed attempts at the same fix or when evidence surprises you. Skip it for simple tasks.

## Where the idea comes from
Carhart-Harris's entropic brain hypothesis (2014) and his REBUS model with Karl Friston (2019) propose that high-level beliefs normally carry heavy weight and constrain what lower levels report. Psychedelics relax that weight, so bottom-up information flows more freely. The authors compare this to annealing: heat lets a system leave a stuck state, and cooling lets it settle into a new one. The same loosening also makes false insight more likely, which is why integration afterward matters.

Vervaeke notes that the pattern finding that makes us adaptive also locks us in. In the nine dot problem, people fail because they project a square that is not in the data. Breaking a frame is not enough; you must also build a better one, and move between the two. Breaking alone leads to choking, and building alone leaps into a wrong frame and fixation. Telling people to think outside the box does not help them; a practice does. That is why this skill is a set of steps, not a reminder.

## Where it may not transfer
- REBUS describes brains. Claude has no confidence dial to turn down. Writing the belief as one candidate is a procedure, not a change of internal state.
- The old belief stays in context and can still steer the reading. Marking skipped evidence in step 2 is the guard, not a guarantee.
- Generated alternatives can be one idea reworded. Asking for differences in kind makes this visible but does not prevent it.
- The insight research is on humans solving puzzles. Whether a written version helps a language model as much is untested.