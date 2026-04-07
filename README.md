# Cognitive Security Chapter Working Guide

This repository is the working space for a contributed textbook chapter for Cognitive Security: Resilient Decision-Making in the Information Age. The chapter is expected to translate existing papers, reports, and figures into a coherent, undergraduate-accessible treatment of formal methods in cognitive security, with room for clearly marked advanced technical material.

The current working theme is formal methods for cognitive security, centered on engagement, gaze, and cybersickness models and the guarantees or evaluation methods that make those models trustworthy. This README is the coordination brief for the team until the main draft in chapter_tex/chapter_author.tex is fully populated.

## Chapter Mission

The chapter should do more than survey prior work. It should explain why the relevant effects and protections occur, how formal or semi-formal models help reason about them, and where the limits of current methods remain. The textbook guidance emphasizes critical thinking, theory-neutral framing where possible, practical relevance, and a global perspective.

For this chapter, that means:

- define what cognitive security means in this modeling context
- explain why formal methods are useful for reasoning about cognitive-state-related risks and interventions
- connect mathematical or computational models to concrete cognitive security problems rather than presenting methods in isolation
- keep the main narrative readable for undergraduate and early graduate students
- isolate advanced proofs, guarantees, or deeper technical details into clearly marked technical subsections or boxes

## What This Chapter Should Answer

The editors asked each chapter to address as many of the following questions as are relevant to the domain. This chapter should explicitly cover them where possible:

1. How is cognitive security defined in this domain?
2. What are the primary theories or modeling traditions in this domain, and what assumptions do they make?
3. What seminal studies, effects, or results support those theories?
4. What methodologies are commonly used?
5. How does this topic integrate with other cognitive security domains?
6. What are the main limitations of current theories and methods, and how might they be overcome?
7. What other technical or operational challenges remain?
8. What future directions, technological changes, or societal shifts are likely to change the landscape?

## Cross-Cutting Textbook Themes

The textbook guidance also asks authors to align with broader cross-chapter questions. This chapter should address the following where relevant:

- the role of individual differences in behavior, response, or vulnerability
- the role of trust and credibility, including how those terms are being used
- the distinction between resilience and mitigation
- how readers can apply the chapter's ideas in practice

The policy-focused prompts in the textbook guidance, such as state versus non-state actors or legal issues, are optional unless the final scope of the chapter expands into policy or international relations.

## Recommended Chapter Structure

The authoritative chapter draft should live in chapter_tex/chapter_author.tex, but the team should write toward a stable structure early. A recommended outline is below.

| Section                                      | Purpose                                                                                                         | Likely Inputs                                                     |
| -------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Introduction and motivation                  | Define the problem, explain why formal methods matter for cognitive security, and establish the chapter's scope | invitation email, textbook guidance, framing from existing papers |
| Foundations and modeling lens                | Introduce formal methods, modeling assumptions, and the chapter's interpretation of cognitive security          | chapter synthesis, prior reports, foundational references         |
| Engagement models                            | Explain engagement-related modeling approaches, what they predict, and why they matter                          | papers/C_EngagementPredictionForMR_IEEEVR_2026 (6).pdf            |
| Gaze and related formalization               | Explain gaze-related observables or state inference if included in the final scope                              | current and future papers in papers/                              |
| Cybersickness models and guarantees          | Explain cybersickness modeling, validation, uncertainty, and any guarantee language the team can defend         | papers/cybersickness_model_202510 (3).pdf                         |
| Quantitative, qualitative, or hybrid methods | Explain the kinds of modeling approaches used and why they are appropriate                                      | chapter synthesis, sample Greitzer chapter structure              |
| Evaluation, guarantees, and limitations      | Describe validation strategies, performance metrics, guarantees, assumptions, and failure modes                 | current papers, formal methods framing, sample chapter pattern    |
| Applications to cognitive security           | Tie the models back to resilient decision-making, intervention design, or operator support                      | chapter synthesis                                                 |
| Open problems and future directions          | Identify unresolved technical and conceptual gaps                                                               | chapter synthesis, editor guidance                                |
| Key points and end-of-chapter questions      | Provide takeaways and questions suitable for teaching                                                           | final editorial pass                                              |

The current Springer template already expects key points, questions, further reading, and references. The sample insider-risk chapter in the repo is a useful structural example for how to combine foundations, modeling approaches, evaluation, and end-of-chapter teaching material.

## Deliverables

The finished chapter package should include the following:

- approximately 8000 words of main chapter content
- a one-page abstract for topic deconfliction or editor coordination if still requested
- a complete LaTeX draft in chapter_tex/chapter_author.tex
- a populated shared bibliography in chapter_tex/references_chapter.bib
- figures and tables reused or adapted from existing papers and reports where licensing and authorship allow
- 3 to 5 key takeaways for the end of the chapter
- 5 to 10 end-of-chapter questions
- optional interactive or multimedia supplements only if the team decides they are worth the extra effort

## Rules and Constraints

- Write for undergraduate and early graduate readers first.
- Keep the main narrative explanatory rather than purely taxonomic.
- Use advanced technical modules only where they improve rigor without breaking accessibility.
- Ground claims in cited papers, reports, or other traceable evidence.
- Reuse existing papers, reports, and figures where appropriate so effort stays focused on synthesis rather than reinvention.
- Keep definitions and terminology consistent with broader cognitive security themes where possible.
- Stay theory neutral and politically neutral where feasible.
- Separate well-supported claims from speculative future directions.
- Treat guarantee language carefully. Only claim formal guarantees, validation strength, or robustness properties that the team can defend from the source material.
- Assume the extracted guidance is correct for planning, but spot-check the original PDF if exact wording becomes important.

## Current Source Materials

The repository already contains a small but growing source base.

- chapter_tex/chapter_author.tex: Springer chapter template that will become the main draft
- chapter_tex/references_chapter.bib: shared bibliography file
- Cognitive_Security_Textbook_Guiding_Principles.pdf: editor guidance for chapter goals and common questions
- Greitzer-Chapter-Science-of-InsThrt.docx: sample science-oriented chapter structure with foundations, models, metrics, key points, and questions
- papers/C_BayesianNetworkForVR_ISMAR_2025 (2).pdf: likely source for formal or probabilistic modeling content
- papers/C_EngagementPredictionForMR_IEEEVR_2026 (6).pdf: likely source for engagement modeling content
- papers/cybersickness_model_202510 (3).pdf: likely source for cybersickness modeling content

As new papers are added, update this README if they materially change scope or add a new workstream.

## Work Split

Use workstreams rather than named ownership in this document. Named assignments can be decided separately.

| Workstream                                | Scope                                                                                 | Expected Output                                               |
| ----------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------- |
| Chapter architecture and synthesis        | unify the chapter thesis, outline, and cross-section consistency                      | stable outline, section goals, integration notes              |
| Formal methods foundations and guarantees | explain the modeling lens, formal reasoning, assumptions, and guarantee language      | foundation section, guarantee terminology, limitations notes  |
| Engagement modeling evidence              | extract claims, methods, figures, and limits from engagement-related papers           | draft subsection text, candidate figures, citations           |
| Gaze modeling and formalization           | extract gaze-related modeling or inference content as papers are added                | subsection notes, citations, open gaps                        |
| Cybersickness modeling                    | extract the key models, metrics, and implications from cybersickness papers           | subsection text, candidate figures, citations                 |
| Evaluation and metrics                    | define how the chapter discusses performance, validation, uncertainty, and comparison | metrics subsection, evaluation table ideas                    |
| Figures and tables                        | decide which visuals to reuse, redraw, or combine                                     | cleaned figure list, caption drafts, permissions check        |
| Bibliography and citation cleanup         | maintain the shared BibTeX file and citation consistency                              | updated references_chapter.bib, missing citation list         |
| Pedagogy and readability review           | keep the chapter accessible to the intended audience                                  | simplification edits, glossary suggestions, question drafts   |
| LaTeX integration and final assembly      | merge the material into the Springer template and keep structure consistent           | integrated chapter draft, section labels, compiled references |

Some workstreams can proceed in parallel immediately: engagement, gaze, cybersickness, bibliography cleanup, and figure inventory. The architecture, guarantees framing, and final assembly workstreams should run continuously but will require later synthesis once the evidence sections are drafted.

## Repository Workflow

Use the repository consistently to avoid fragmented drafts.

- README.md is the planning and coordination document.
- chapter_tex/chapter_author.tex is the authoritative chapter draft target.
- chapter_tex/references_chapter.bib is the shared bibliography source for citations.
- papers/ is the source-material inventory, not the place for draft prose.
- Binary guidance documents can be referenced for planning, but implementation should happen in markdown or LaTeX files inside the repo.

Recommended workflow:

1. Agree on a stable chapter scope and a short abstract.
2. Extract claims, figures, equations, and citations from current papers into notes or directly into the chapter draft.
3. Expand the bibliography as each source is adopted.
4. Draft subsection content in chapter_tex/chapter_author.tex against the agreed structure.
5. Add key points, questions, and further reading after the technical narrative is stable.
6. Perform a consistency pass on terminology, cross-references, figures, and citations.

## Milestones and Sequence

The team note suggests aiming for a first draft in May. A practical sequence is:

1. Confirm chapter scope, provisional title, and one-page abstract.
2. Partition the work into the workstreams above.
3. Mine current papers for reusable claims, figures, and citations.
4. Build a stable section outline and identify missing evidence.
5. Draft the main sections in LaTeX.
6. Add evaluation, limitations, and future directions once the evidence sections exist.
7. Draft key points and end-of-chapter questions.
8. Clean up references, captions, and terminology.
9. Review the draft against the textbook guidance before circulation.

## Known Limitations and Pending Decisions

- The final chapter title is still provisional.
- Final author order and named ownership are not yet captured here.
- The papers directory will likely keep growing, so the outline may need to absorb additional evidence.
- The guidance documents were converted from binary files, so exact publisher wording should be checked against the originals if a wording-sensitive decision arises.
- The current LaTeX file is still a Springer sample template and will need substantial replacement rather than incremental polishing.

## Definition of Done for the README

This README is doing its job if a collaborator can open the repository and quickly answer the following:

1. What is this chapter trying to do?
2. What questions should the chapter answer?
3. What deliverables are expected beyond prose?
4. What rules and limitations should shape the writing?
5. Where in the repo should each kind of work happen?
