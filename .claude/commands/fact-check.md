Go over the content of `1-clean.md` in the current directory in detail. Your job is to verify every factual claim, fill in any blanks (e.g. sections marked "todo: add information on X"), and produce `2-fact-checked.md`.

## Process

For each factual claim or statement that could be verified:

1. Use subagents to research the subject thoroughly — do not jump to conclusions
2. Each subagent should save its findings and references as a markdown file in the same directory (e.g. `research-[topic].md`)
3. Once all research is done, categorise each claim as below

### If the content is clearly correct

Add a reference if the claim is the kind that could be challenged or questioned — for example, specific dates, percentages, named effects, attributed quotes, or causal claims. General knowledge (e.g. "practice helps learning") does not need a reference, but specific claims (e.g. "spaced repetition improves retention by 50%") do.

There might be a common misunderstanding worth pointing out to readers. Offer to include a brief note on the common misconception.

### If the content is clearly INCORRECT

Explain what is incorrect and why, and ask the user how to proceed. If corrections are made, include references using the **references** skill.

### If the content is controversial (unclear if correct or incorrect)

Ask the user if it should be treated as correct or incorrect. The user might also choose to include both perspectives.

## Filling in blanks

If any section contains placeholders like "todo: add information on X":
1. Use subagents to research the topic
2. Write the content following the **voice-and-tone** skill
3. Include references using the **references** skill

## Reference format

Follow the **references** skill for all inline citations and the bottom references section.

## In all cases

- Web research is required — do not rely on assumptions
- Do not invent research findings or statistics
- Every challengeable fact must have a reference. A "challengeable fact" is any claim a skeptical reader might ask "source?" about — specific numbers, dates, effect sizes, named studies, attributed ideas, or causal statements. If you cannot find a credible source for a claim, flag it to the user rather than leaving it unreferenced.
- Write the final output to `2-fact-checked.md`