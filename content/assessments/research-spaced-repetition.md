# Research Notes: Spaced Repetition and Long-Term Retention

## The Core Claim

A learner who answers correctly once -- on a quiz, in a discussion, or during practice -- may not retain that knowledge days or weeks later. A single correct response is not evidence of durable learning. Spaced repetition (revisiting material at increasing intervals over time) is one of the most well-supported strategies in cognitive science for building long-term retention.

---

## The Forgetting Curve (Ebbinghaus, 1885)

Hermann Ebbinghaus conducted the original experimental work on memory from 1880 to 1885, memorising nonsense syllables and testing himself after various delays. He found that **memory loss follows an exponential pattern**: most forgetting happens soon after learning, and the rate of loss gradually slows. Crucially, he also found that each repetition flattened the forgetting curve -- the same material was retained longer after each review.

A 2015 replication by Murre and Dros confirmed Ebbinghaus's original findings using modern methods.

- Murre, J. M. J., & Dros, J. (2015). Replication and Analysis of Ebbinghaus' Forgetting Curve. *PLOS ONE*. [https://pmc.ncbi.nlm.nih.gov/articles/PMC4492928/](https://pmc.ncbi.nlm.nih.gov/articles/PMC4492928/)
- Wikipedia overview of the forgetting curve: [https://en.wikipedia.org/wiki/Forgetting_curve](https://en.wikipedia.org/wiki/Forgetting_curve)

---

## The Testing Effect (Roediger & Karpicke, 2006)

This is the finding most directly relevant to the claim. Roediger and Karpicke had students either restudy a prose passage multiple times or take recall tests on it (without feedback). The results:

- **After 5 minutes**, the restudy group performed better.
- **After 2 days**, the testing group dramatically outperformed the restudy group.
- The restudy group forgot **56%** of what they originally recalled, while the repeated-testing group forgot only **13%**.

The takeaway: retrieving information from memory (not just re-reading or re-hearing it) strengthens the memory trace far more than passive review. A single correct answer during initial learning does not protect against later forgetting -- but repeated retrieval over time does.

- Roediger, H. L., & Karpicke, J. D. (2006). Test-Enhanced Learning: Taking Memory Tests Improves Long-Term Retention. *Psychological Science*, 17(3), 249--255. [https://pubmed.ncbi.nlm.nih.gov/16507066/](https://pubmed.ncbi.nlm.nih.gov/16507066/)
- Full text PDF: [https://gwern.net/doc/psychology/spaced-repetition/2006-roediger.pdf](https://gwern.net/doc/psychology/spaced-repetition/2006-roediger.pdf)

---

## The Spacing Effect (Cepeda, Pashler, Vul, Wixted & Rohrer, 2006; 2008)

A meta-analysis of **839 assessments across 317 experiments** confirmed the spacing effect: distributing study sessions over time reliably improves recall compared to massing them together (cramming).

A follow-up study with over 1,350 participants found that the **optimal spacing gap depends on how long you need to remember**. For a test a few weeks away, the optimal review gap was roughly 20% of the retention interval. For retention over a year, the optimal gap dropped to about 5% of that interval -- but still required multiple spaced reviews.

- Cepeda, N. J., Pashler, H., Vul, E., Wixted, J. T., & Rohrer, D. (2006). Distributed Practice in Verbal Recall Tasks: A Review and Quantitative Synthesis. *Psychological Bulletin*, 132(3), 354--380. [https://pubmed.ncbi.nlm.nih.gov/16719566/](https://pubmed.ncbi.nlm.nih.gov/16719566/)
- Cepeda, N. J., Vul, E., Rohrer, D., Wixted, J. T., & Pashler, H. (2008). Spacing Effects in Learning: A Temporal Ridgeline of Optimal Retention. *Psychological Science*, 19(11), 1095--1102. [https://pubmed.ncbi.nlm.nih.gov/19076480/](https://pubmed.ncbi.nlm.nih.gov/19076480/)
- Full text PDF of the 2008 study: [https://laplab.ucsd.edu/articles/Cepeda%20et%20al%202008_psychsci.pdf](https://laplab.ucsd.edu/articles/Cepeda%20et%20al%202008_psychsci.pdf)

---

## Practical Consensus (Dunlosky et al., 2013)

A landmark review evaluated 10 common learning techniques for their effectiveness. Out of all techniques reviewed, only two received the highest "high utility" rating:

1. **Practice testing** (retrieval practice)
2. **Distributed practice** (spaced repetition)

Popular techniques like highlighting, rereading, and summarisation were rated as low utility. The authors noted that spaced practice and retrieval practice are effective across many domains and populations, are relatively easy to implement, and do not require extensive training.

- Dunlosky, J., Rawson, K. A., Marsh, E. J., Nathan, M. J., & Willingham, D. T. (2013). Improving Students' Learning With Effective Learning Techniques. *Psychological Science in the Public Interest*, 14(1), 4--58. [https://journals.sagepub.com/doi/abs/10.1177/1529100612453266](https://journals.sagepub.com/doi/abs/10.1177/1529100612453266)
- Dunlosky, J. (2013). Strengthening the Student Toolbox. *American Educator*, Fall 2013. [https://www.aft.org/ae/fall2013/dunlosky](https://www.aft.org/ae/fall2013/dunlosky)

---

## Summary for the Workbook

The research strongly supports three linked claims:

1. **Forgetting is rapid and predictable.** Without review, most of what someone learns is forgotten within days (Ebbinghaus; Murre & Dros, 2015).

2. **A single correct response is not durable learning.** Learners who answered correctly via restudy forgot 56% within two days; those who practised retrieval forgot only 13% (Roediger & Karpicke, 2006).

3. **Spaced retrieval practice is the most effective countermeasure.** Reviewing material at increasing intervals -- not just once, but multiple times over days and weeks -- is one of only two learning techniques rated "high utility" across a comprehensive review of the evidence (Dunlosky et al., 2013; Cepeda et al., 2006, 2008).

For training designers, this means: do not assume that learners who perform well during a session will retain that knowledge. Build in spaced review opportunities -- follow-up quizzes, reflection prompts, or brief recap activities days and weeks after initial instruction.
