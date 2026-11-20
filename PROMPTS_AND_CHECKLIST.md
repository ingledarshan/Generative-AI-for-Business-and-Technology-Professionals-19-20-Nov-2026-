# Lab 1 — Copy-and-Paste Prompts and Evaluation Checklist

## Prompt 1 — Generate the first artifact

Act as an IT Operations Analyst. Find and activate the `weekly-incident-report` Skill and follow its instructions.

**Business requirement:** An operations manager needs a professional one-page weekly incident report to identify where to focus operational review.

**Source:** `Walmart GenAI Course/Lab Files/Weekly Incidents.txt`
**Audience:** IT operations manager
**Output:** `Walmart GenAI Course/Lab Files/Weekly_Incident_Brief.md`

Include a brief executive summary, accurate KPI and regional tables, evidence-based observations, no more than three practical recommendations, and explicit missing-data limitations. Show total incidents and scanner-sync incidents without double-counting. Calculate percentages using the correct denominator.

Use only the specified local dataset. Do not invent incident severity, root causes, trend comparisons, or customer impact. Do not alter the source file or other files, run unnecessary commands, or access the internet. You may create the single requested Markdown output file. At the end, explain what you created and which facts you verified.

## Prompt 2 — Iterative refinement

Review the Markdown report you just created against the original `Weekly Incidents.txt` file and the `weekly-incident-report` Skill. Improve the **same report**, not a new file:

1. Make the executive summary shorter and clearer for an operations manager.
2. Ensure every percentage states its numerator and denominator.
3. Distinguish observed facts from recommendations.
4. Clearly say that one week's data cannot establish a trend or root cause.
5. Keep the document concise and readable.

Do not alter any numeric source data or other files. After updating, tell me exactly what changed.

## Prompt 3 — Independent quality review

Act as a strict quality reviewer. Compare `Walmart GenAI Course/Lab Files/Weekly_Incident_Brief.md` with `Walmart GenAI Course/Lab Files/Weekly Incidents.txt`.

Score the report out of 5 for completeness, accuracy, relevance, and transparency. For each criterion provide a one-sentence justification and identify any unsupported statement or number. Do not edit files. Conclude with PASS or REVISE and explain why.

## Participant validation checklist

- [ ] The report uses the specified week and names the source.
- [ ] The total incidents count matches the dataset.
- [ ] Scanner-sync incidents are treated as a subset, not added to totals.
- [ ] Regional counts and percentages are mathematically correct.
- [ ] There are no made-up incident categories, root causes, or trends.
- [ ] Missing severity, priority, incident-level details and customer impact are disclosed where absent.
- [ ] Recommendations are plausible next steps, not unsupported factual claims.
- [ ] The artifact can be read by a nontechnical operations manager.

## Trainer discussion prompts

- What improved when we added a Role, Source, Output and Constraints?
- What does the Skill standardize that the one-time prompt does not?
- Why is a polished report still not automatically a reliable report?
