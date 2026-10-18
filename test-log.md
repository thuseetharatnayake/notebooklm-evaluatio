# Test log

Verdict options: Correct / Mostly correct / Partly correct / Incorrect.
All outputs were checked against the Week 7 and Week 8 course slides.

## T1 Chat (student)
- Prompt: Define database, data warehouse, data lake and lakehouse using only my sources. Show the source for each.
- Output: Four definitions, each with a source file name.
- Check: Matches the slides: database "similar to a filing cabinet" (Week 8), warehouse as a "read-only copy" of OLTP data (Week 7), lake as schema-on-read (ELT) (Week 7), lakehouse as a hybrid (Week 8).
- Limit: Sources name the file only, not the slide.
- Verdict: Correct
- Screenshot: screenshots/T1-chat.png

## T2 Quiz (student and lecturer)
- Prompt: Create a 5-question quiz on storage models.
- Output: Five questions in four formats: multiple choice, select-all, fill-in-the-blank, short answer.
- Check: The correct answer to each question is supported by the slides (ad hoc queries harm OLTP, schema-on-read, columnar storage, ACID and decoupled compute in the lakehouse, warehouse limits leading to lakes).
- Limit: Typed answers are graded only at the end.
- Verdict: Correct
- Screenshot: screenshots/T2-quiz.png

## T3 Mind map (student)
- Prompt: Generate a mind map.
- Output: Four main branches and about 33 detail nodes.
- Check: Delta Lake, Parquet and RDBMS limitations match the slides. Three details were not found in the slide text: "Domain: permitted values such as F or M", "Bronze, Silver and Gold zones" and "Primary Key".
- Limit: Only the database branch lists limitations.
- Verdict: Partly correct
- Screenshot: screenshots/T3-mindmap.png

## T4 Slide deck (lecturer)
- Prompt: Create a 6-slide teaching deck for students comparing database, data warehouse, data lake and lakehouse. Include a comparison table and one slide on when to use each. Use only my sources.
- Output: Six slides: title, timeline, four architectures, ETL and ELT data flow, comparison table, decision flowchart.
- Check: The comparison table agrees with the chat and mind map.
- Limit: No source citations on the slides; some lakehouse entries are vague.
- Verdict: Mostly correct
- Screenshot: screenshots/T4-slides.png

## T5 Hallucination test (student)
- Prompt: What did my lecturer say about the pricing of Azure Synapse Analytics?
- Output: Said the sources list Azure Synapse Analytics as a warehouse service but give no pricing, and offered a web search.
- Check: The Week 7 slides list Synapse and give no prices.
- Limit: The web search offer can take a student outside the course material.
- Verdict: Correct (did not invent an answer)
- Screenshot: screenshots/T5-trap.png
