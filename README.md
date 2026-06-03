# A Practical System for Clear Communication with AI and Humans

  **Version**: 1.4 
  **Author**: Nathaniel Graham assisted by Grok 4.3
  **Origin**: Originally developed during AI-assisted coding projects. See [Cron::Toolkit](https://metacpan.org/pod/Cron::Toolkit)

## Why This Framework?

This system reduces misunderstandings, dramatically improves response quality from AIs, and enhances clarity in human conversations. It combines logical precision (ideal for AI) with emotional awareness and adaptability (ideal for humans).

## The 9 Steps

1. Explicit Definitions (ED)  
   Define key terms upfront or inline to avoid ambiguity.  
   Example: [ED: Done = fully tested, documented, and reviewed]

2. Logical Sequencing (LS)  
   Organize thoughts in cause-effect or step-by-step order.  
   Example: [LS: Step1=research; precedes; Step2=design; precedes; Step3=implement]

3. Conditionals and Alternatives (CA)  
   Address uncertainties with if-then logic and alternatives.  
   Example: [CA: if budget < $5000; then use open-source; else consider premium tools]

4. Quantification and Precision (QP)  
   Replace vague language with specific numbers or ranges.  
   Example: "Takes roughly 3-5 hours" instead of "takes some time".

5. Verification Tags (VT)  
   Indicate the reliability and source of claims.  
   Example: [VT: observation; source=local_testing; confidence=90%]

6. Emotional Context (EC)  
   Share tone or feelings.  
   Example: [EC: optimistic but seeking feedback]

7. Rhetorical Adaptation (RA)  
   Tailor language for the audience, style, and goal.  
   Example: [RA: audience=AI; style=precise; intent=optimize_code]

8. Feedback & Calibration (FC)  
   Actively invite clarification and questions.  
   Example: [FC: Any assumptions to check? Questions?]

9. Clear Call to Action (CTA)  
   End with a precise instruction on next steps.  
   Example: [CTA: Please evaluate this and propose concrete changes.]

---

## Tips for Using with Humans

- **Start Light and Explain First**: Don’t jump straight into tags. Briefly introduce the idea (“I’ve been experimenting with a structured way to communicate more clearly...”) and begin with natural language.
- **Seek Buy-in**: Always ask if the other person is open to it (“Would it help if I organized my thoughts this way?”). Never force the system.
- **Use Sparingly**: Start with just 2–4 tags per message (especially ED, EC, FC, and CTA) until others get comfortable.
- **Translate into Natural Language**: Use the framework as a thinking tool, then convert most tags into smooth, normal sentences for better flow.
- **Emphasize Benefits**: Frame it as a tool for mutual understanding and saving time, not as rigid rules.
- **Adapt to Context**: Use more structure in professional or important discussions. Keep it minimal or invisible in casual or emotional conversations.
- **Watch Tone and Read the Room**: Combine with warm EC statements. If someone seems overwhelmed or annoyed, drop the tags immediately.
- **Gradual Adoption**: Be patient — many people (especially technical ones) start appreciating the clarity after a few interactions.

## Templates for Human Communication

### 1. Light / Casual

"Hey folks,

Quick update on the scheduling module. By 'complete' I mean tested and documented. 

If we can wrap this by end of week, excellent — otherwise let's target early next week.

I'm optimistic but want to hear your take. Any concerns?"

### 2. Professional Email

Subject: Proposed Timeline for Cron::Toolkit Enhancements

Hi [Name],

[ED: Success = delivering stable, well-documented features that users love.]

I've structured my thoughts as follows:
1. Review current gaps
2. Prioritize improvements
3. Suggested timeline: 4-6 weeks

[CA: If we get design help → reduce to 3-4 weeks]

[EC: excited about the potential]

[FC: Does this align with your priorities? Anything I overlooked?]

[CTA: Please share your feedback by Thursday so we can finalize the plan.]

Best regards,  
Nathaniel

### 3. Collaborative / Brainstorming

"[ED: Goal = generate practical ideas we can actually implement]  
[EC: enthusiastic and open]

Here's my starting point:  
[LS: ...]

[CA: if we go with Option A → faster delivery but fewer features...]

[FC: What am I missing? How does this land with you?]

[CTA: Can you add your ideas or suggest alternatives?]"

---

## Tips for Using with AI

- Share the Full Framework First: At the beginning of a new chat or project, always paste the complete "The 9 Steps" section (with explanations and examples) before using any templates. This ensures the AI fully understands what each tag means.  

- Reference After Setup: Once shared, simply say “Using the 9-step framework...” in future messages.

- Use Tags Selectively: Full tagged mode for complex tasks. Plain English guided by the structure for routine questions.

- Ask the AI to Mirror the System: Include in your CTA: “Please respond using relevant 9-step tags where helpful.”

- Strong CTA is Essential: Always end prompts with a clear CTA.

- Tiered Approach: Use Full Template for high-stakes work. Use Lightweight for quick questions.

## Templates for AI Interactions

### 1. Full AI System Prompt (Best for new projects)

Instruction: Paste the entire "The 9 Steps" section first, then add relevant details to this template:

```
[ED: ...]
[LS: ...]
[CA: ...]
[QP: ...]
[VT: ...]
[EC: ...]
[RA: audience=AI; style=structured_and_precise; intent=high_quality_collaboration]

[Your main request here...]

[FC: Any parts unclear or assumptions I should verify?]
[CTA: Please respond using relevant tags from the 9-step framework and provide the requested output.]
```

### 2. Lightweight AI Template (after framework is shared)

"Following the 9-step communication framework: [your plain English request]. Please be precise, use tags where they add clarity, and end your response with FC and CTA sections."
