# Content Workflow

We use a series of Claude Code commands to turn a rough draft into a complete workbook chapter. The user provides a file called `0-rough.md`, then runs each command in order, reviewing and adjusting the output between steps.

## Pipeline

### Step 1: /fix-tone-and-structure
Input: 0-rough.md
Output: 1-clean.md
Get the tone and structure right.

### Step 2: /fact-check
Input: 1-clean.md
Output: 2-fact-checked.md
Check all facts. Fill in any blanks (e.g. sections marked "todo: add information on X") using subagents.

### Step 3: /glossary
Input: 2-fact-checked.md
Output: 3-glossary.md
Add a glossary of key terms introduced in the chapter.

### Step 4: /make-preamble
Input: 3-glossary.md
Output: 4-preamble.md
Create up-front learning outcomes and questions.

### Step 5: /add-remember-boxes
Input: 4-preamble.md
Output: 5-remember.md
Add callout boxes to highlight key takeaways the reader should remember.

### Step 6: /suggest-activities
Input: 5-remember.md
Output: 6-activities.md
Suggest self-study activities for the workbook. Readers do these on their own, applying concepts to their own content or learners.

### Step 7: /workshop-activities
Input: 6-activities.md
Output: workshop-activities.md (separate file, not part of the main pipeline)
Suggest group activities for live classroom workshops. This is a standalone output used in a different workflow.

### Step 8: /extra-readings
Input: 6-activities.md
Output: 7-readings.md
Add extra readings and references.

### Step 9: /consistency-pass
Input: 7-readings.md
Output: 8-complete.md
Final consistency pass across the whole chapter: check formatting, terminology, tone, and cross-references.

# Some extra commands for bulletproofing

## /harden-outcomes
Input: 8-complete.md
Output: 8-complete.md
Make a map of outcomes, exercises and their bloom levels and make sure there are no gaps or misalignments


## harden-workshop-activities

Input: workshop-activities.md
Output: workshop-activities.md

