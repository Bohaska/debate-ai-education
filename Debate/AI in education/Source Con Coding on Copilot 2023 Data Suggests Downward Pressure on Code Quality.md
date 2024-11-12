Title: Coding on Copilot: 2023 Data Suggests Downward Pressure on Code Quality (Incl 2024 Projections)
Link: https://www.gitclear.com/coding_on_copilot_data_shows_ais_downward_pressure_on_code_quality
Citation:
> [!note] Citation
> ## GitClear 2024
> Harding, William, and Matthew Kloster. “Coding on Copilot: 2023 Data Suggests Downward Pressure on Code Quality (Incl 2024 Projections).” GitClear, January 16, 2024. [https://www.gitclear.com/coding_on_copilot_data_shows_ais_downward_pressure_on_code_quality](https://www.gitclear.com/coding_on_copilot_data_shows_ais_downward_pressure_on_code_quality).

# Abstract
2023 marked the coming out party for GitHub Copilot. In less than two years’ time, the AI programming assistant shot from “prototype” to “cornerstone,” used by millions of developers across hundreds of thousands of businesses [1]. Its unprecedented growth defines a new era in “how code gets written.” 

GitHub has published several pieces of research on the growth and impact of AI on software development. Among their findings is that developers write code “55% faster” when using Copilot. This profusion of LLM-generated code begs the question: how does the code quality and maintainability compare to what would have been written by a human? Is it more similar to the careful, refined contributions of a Senior Developer, or more akin to the disjointed work of a short-term contractor? 

To investigate, GitClear collected 153 million changed lines of code, authored between January 2020 and December 2023 [A1]. This is the largest known database of highly structured code change data that has been used to evaluate code quality differences [A2]. 

We find disconcerting trends for maintainability. Code churn -- the percentage of lines that are reverted or updated less than two weeks after being authored -- is projected to double in 2024 compared to its 2021, pre-AI baseline. We further find that the percentage of "added code" and "copy/pasted code" is increasing in proportion to “updated,” “deleted,” and “moved” code. In this regard, code generated during 2023 more resembles an itinerant contributor, prone to violate the DRY-ness of the repos visited. 

We conclude with suggestions for managers seeking to maintain high code quality in spite of the momentum opposing that goal.

**Churn increased by 39% (Churn is defined by percentage of code which was reverted in less than 2 weeks)**