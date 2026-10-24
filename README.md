# A Practical System for Clear Communication with AI and Humans

Originally developed with assistance from Grok during a coding project, this framework is now used primarily as a tool for clarifying one’s own thinking across domains. It remains useful for communication with agents and (more cautiously) with other humans.

The nine steps below are still the full set. In practice, only a subset is usually needed.

# The 9 Steps

1. Explicit Definitions (ED)  
   Define key terms upfront or inline to avoid ambiguity.  
   Example: [ED: Done = fully tested, documented, and reviewed]  
   Note: With humans this can sometimes feel condescending even when unintended. Use sparingly and prefer plain phrasing (“when I say done I mean…”) over a labeled tag.

2. Logical Sequencing (LS)  
   Organize thoughts in cause-effect or step-by-step order.  
   Example: [LS: Step1=research; precedes; Step2=design; precedes; Step3=implement]

3. Conditionals and Alternatives (CA)  
   Address uncertainties with if-then logic and alternatives.  
   Example: [CA: if budget < $5000; then use open-source; else consider premium tools]

4. Quantification and Precision (QP)  
   Replace vague language with specific numbers or ranges.  
   Example: “Takes roughly 3–5 hours” instead of “takes some time”.

5. Verification Tags (VT)  
   Indicate the reliability and source of claims.  
   Example: [VT: observation; source=local_testing; confidence=90%]  
   With agents this improves inspectability and can slightly reduce confident overclaiming, but does not strongly prevent hallucinations on its own. Agents can still mislabel the epistemic status. Most useful for factual or research-style work; lower priority than ED, FC, and CTA for routine tasks.

6. Emotional Context (EC)  
   Share tone or feelings.  
   Example: [EC: optimistic but seeking feedback]

7. Rhetorical Adaptation (RA)  
   Tailor language for the audience, style, and goal.  
   Example: [RA: audience=AI; style=precise; intent=optimize_code]

8. Feedback & Calibration (FC)  
   Actively invite clarification and questions.  
   Example: [FC: Any assumptions to check? Questions?]  
   Especially important with agents: without an explicit invitation to ask, they will usually fill gaps with assumptions rather than clarify. Still useful with humans, but keep the phrasing low-pressure.

9. Clear Call to Action (CTA)  
   End with a precise instruction on next steps.  
   Example: [CTA: Please evaluate this and propose concrete changes.]

---

## Current Usage Priorities

**Self-thinking (primary use):**  
Any of the steps can help, depending on the problem. ED, LS, CA, and QP are the ones most often applied privately to force clearer reasoning before speaking or writing.

**With agents:**  
ED, FC, and CTA are the high-value core.  
- ED reduces invented definitions.  
- FC is non-optional in collaborative or multi-turn work; agents default to assuming rather than asking.  
- CTA keeps the output bounded and actionable.  
The remaining steps can be added when useful but are not required once these three are solid. VT is optional and mainly improves inspectability of factual claims.

**With humans:**  
LS, FC, and CTA, used lightly. ED only when a term is genuinely contested or high-stakes, and preferably without the tag.  
Some people read explicit definitions or visible structure as talking down to them. Keep tags (and even the visible discipline) minimal, frame any structure as “here’s how I’m thinking about it,” and drop it immediately if the other person seems uncomfortable. Plain language that is precise often works better than labeled steps.

---

## Tips for Using with Humans

- Start light. Do not open with tags. Use ordinary language first.
- ED is higher-risk than the other steps. Prefer “when I say X I mean…” or simply using the precise term without calling it a definition. Labeled ED blocks are more likely to land as condescending.
- Prefer LS, a light FC, and a clear CTA. Keep even those mostly invisible.
- Translate structure into normal sentences. Use the framework as a thinking tool, then write naturally.
- Watch the room. If someone seems annoyed or confused by the structure, stop using tags at once.
- A plain “Any assumptions I should check?” still helps without sounding systematic.

## Tips for Using with Agents

- Share the framework (or at least the relevant steps) once at the start of a project or long thread if you want the agent to mirror the style.
- Treat FC as required for anything collaborative. Explicitly invite questions and assumption checks.
- ED + FC + CTA is usually sufficient. Add others only when they reduce real ambiguity.
- Strong CTAs matter. End with a precise next action.
- After the framework is known, a lightweight prompt is enough: “Following the 9-step framework: [request]. Please flag any unclear points and end with FC and CTA.”

---

## Examples

### Self-thinking / planning note
ED: “Launch-ready” = core flows work, billing is live, and basic docs exist.  
LS: finalize pricing → migrate to VPS → test webhooks → write minimal docs.  
CA: if webhook testing takes >2 days, ship without usage-based limits first.  
CTA: decide on the VPS size by Friday.

### Light human update (no labeled ED)
“Quick update on the scheduling module. By complete I mean tested and documented.  
If we can wrap this by end of week, great; otherwise early next week is fine.  
Any concerns or assumptions I should check?”

### Agent request (core tags)
ED: success = the function handles the three edge cases listed below and includes a short comment on each.  
[main request]  
FC: Any part of the spec unclear or any assumptions you need confirmed before writing code?  
CTA: Please implement the function and note any deviations from the spec.

---

## Templates

### Full (new project or high-stakes, mainly for agents)
Paste the relevant steps (or the full list) first, then:

```
[ED: ...]
[LS: ...]          # optional
[FC: Any assumptions to check? Questions?]
[CTA: ...]

[Your request]
```

### Lightweight (framework already known)
“Following the 9-step framework: [plain-English request]. Flag anything unclear and end with FC and CTA.”
