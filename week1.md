Week: 1/26
Date: 1/30
Talk(s): Papers We Love: No Silver Bullet (conversation with Dr. Fred Brooks)
Questions:
Pre-watch:
How do you anticipate this talk will contribute to your enrichment as a well-rounded practitioner of computer science? (I.e. why did you pick this talk?)
- "Mythical Man Month" is pretty well known within software, and I happen to have read the corresponding essay. I am distanced from the circumstances under which the essay was written by both time (the essay being written 4 decades ago informed by his experiences in the preceeding 3) and by perspective (never having myself been the manager of a multi-billion dollar systems project). Still, I found pieces that were both incredibly salient and also some things that seem accurate today. Having already read the essay while thinking about the present, I hope to listen to the conversation with an eye to the future.
Post-watch:
What did you take away corresponding to your hopes as described above?
- He gave a synopsis which really hammered home the idea that for an advance to increase productivity, it needs to obviate a an subtask--representing a an Aristotelian "accidental complexity," c_a, as opposed to its counterpart, "essential complexity," c_e--which took up a substantial fraction of time. If complexity translates proportionally to time, we can represent max speedup symbolically as 1+c_a/c_e.
- Brooks examined a number of technologies which at the time promised "tenfold" increases in productivity. Today, some have made similar promises about LLMs for programming.
- From a Brooksian lens (and this is all doomed to oversimplification anyway), if one believes that development can be accounted for as the accumulation of code, that 90% of a programmer's activity comprises the typing (and requisite thinking) to produce said code, and that output speed of LLMs will soon become negligable by comparison, this is a cause for optimism. Conversely, the ratio of programming process--be it in planning, thinking, debugging, or otherwise--that LLMs are not capable of reproducing at any point in time (essential complexity) to that which LLMs are (accidental complexity) is one less than the theoretical upper bound on the LLM-driven productivity multiple. 
- I do not pretend to know how large this fraction is or the extent to which it will increase in the future. Still, mainstream discussion so far centers mostly around whether or not LLMs can single shot a given category of output, and would benefit to consider the accidental/essential complexity ratio in the in the concurrent application of LLMs and humans.

What did you take away that you did not anticipate?
- It never really occurred to me that assembly language itself was a productivity multiplier. 
What question(s) do you have, and who do you know that can you ask or explore this with?
- I have a FORTRAN punched card from my grandfather who I unfortunately never met, but I do not really know how punch cards were used. Evidently you could put FORTRAN on them, but I wonder what else went on punch cards, and how we got to stored-program computers (another big program-input productivity boost, I imagine).
