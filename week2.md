Week: 2/2
Date: 2/8
Talk(s): TigerBeetle: Maginal Memory Tour! (Joran Dirk Greef)
Questions:
Pre-watch:
How do you anticipate this talk will contribute to your enrichment as a well-rounded practitioner of computer science? (I.e. why did you pick this talk?)
- When I listed this talk, I had not yet been automatically moved into CS133, so my intent was to preview many of the considerations that go into domain-specific database design.
- As mentioned previously, I am very intrigued the motivations which bring systems designers to eschew dynamic memory allocation, and TigerBeetle is such a system.
Post-watch:
What did you take away corresponding to your hopes as described above?
- Domain specific considerations:
  - Financial databases have very little flexibility in the tradeoff space of generic databases (need perfect reliability, and high performance)
  - Throughput can be increased dramatically if the transaction (that's financial transaction, not CRUD transaction) logic is integrated directly into the database.
  - TigerBeetle makes great use to think of databases as a distributed FSM, which, if deterministic, enables simulation (with injected data corruption and hardware faults) much much faster than real-time, while preserving reproducability. This is critical for TigerBeetle to compete with existing databases that have decades of testing and production use.
  - Motivations for static allocation: Out-of-memory is not something a database can just ignore, so they have to solve resource limitations in one way or another, and they'd rather have control, particularly because it makes testing easier. "What you can't limit, you can't test." Also, (like Hubris), allowing external inputs to cause memory allocation is a security concern.

What did you take away that you did not anticipate?
- I knew that RAFT was easier than PAXOS, but I did not know that some people preferred its ancestor, VSR, in this case for its deterministic properties.
What question(s) do you have, and who do you know that can you ask or explore this with?
- With LLMs as stochastic models, many systems that we are increasingly depending on are decreasingly deterministic, but nevertheless have significant consequences. What are the lessons designers of Information Retrieval systems can learn from TigerBeetle? At work we're doing a little 3-month project about real-time event monitoring for BlueSky, and I lucky enough to be able to bring on a few Mudd-CS peers, we will get many oppportunities to ask ourselves these questions!
