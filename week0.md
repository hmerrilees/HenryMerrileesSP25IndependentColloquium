# Week 0
Week: 1/19
Date: 1/25
Talk(s): On Hubris and Humility: developing an OS for robustness in Rust (Cliff Biffle)

## Questions:
Pre-watch:
- How do you anticipate this talk will contribute to your enrichment as a well-rounded practitioner of computer science? (I.e. why did you pick this talk?)
  - The technical communication in this talk has been described by the speaker's colleagues as "outstanding" and "annoyingly good," which, though I think Hubris/Humility is super cool, is the actual reason I picked the talk and what I hope to learn from.
  - On a technical level, I have an interest in greenfield systems projects which specifically choose to forbid dynamic allocation for the sake of reliability and robustness.
Post-watch:
- What did you take away corresponding to your hopes as described above?
  - The talk is structured almost as though it operates on a call stack. Whenever Cliff dives in enters into a deeper level of abstraction or returns back to a higher level of abstraction, he announces that he is doing so clearly, and prefaces what he intends the listener to learn or to have learned.
  - The talk is willing to dive into rabbit holes but when it does, it stays very focused, and does not get disctracted by the need to cover everything. It chooses its battles.
- What did you take away that you did not anticipate?
  - I've been having a blast with the rust async model recently, and am anticipating doing some async embedded stuff soon. I had previously only considered async weariness at the consumer level of "every time you .await, that's another nested state machine." I had not considered how strongly async OS facilities depend on dynamic allocation in a way that is often infeasible in an embedded context.
- What question(s) do you have, and who do you know that can you ask or explore this with?
  - Re. "don't parse, validate (and use the type system to enforce invariants)", I know Cliff has a more in depth blog about typestates, I can go read about that, and maybe talk about it with Max!
