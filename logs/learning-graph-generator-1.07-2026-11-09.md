# Learning Graph Generator Session Log

- **Skill:** learning-graph-generator v1.07
- **Date:** 2026-11-09
- **Book:** Advanced Topics in Modern Microscopy Techniques (EE 5940)

## Python programs used

| Program | Version | Notes |
|---|---|---|
| csv-to-json.py | 1.05 | Generated `learning-graph.json`, including Concept Impact Scores (CIS) |
| analyze-graph.py | not versioned | Wrote `quality-metrics.md` |
| taxonomy-distribution.py | not versioned | Wrote `taxonomy-distribution.md` |
| validate-learning-graph.py | not versioned | Schema validation, run with the `jsonschema` package |
| add-taxonomy.py | not used | TaxonomyIDs were written directly into the CSV |

The scripts were run with the system Python 3.9. The JSON schema check and the
MkDocs build used a temporary virtual environment with MkDocs 1.6.1,
mkdocs-material and jsonschema.

## Steps

1. **Course description check — skipped.** `docs/course-description.md` already
   had `quality_score: 100`, which is above 85.
2. **Concept list.** Wrote 510 concepts as one spec (label, TaxonomyID, and
   prerequisite labels). A build script checked that every label is 32
   characters or fewer, unique, and that every prerequisite names an earlier
   concept, so the graph cannot contain a cycle. The list was generated end to
   end at the author's request, without a separate review pause.
3. **Dependency graph.** The build script converted prerequisite labels to
   ConceptIDs and wrote `learning-graph.csv` with the TaxonomyID column.
4. **Quality validation.** Valid DAG with 0 cycles and 0 orphaned nodes. There
   are 9 foundational concepts and 147 terminal nodes (28.8%), the average is
   1.68 dependencies per concept, and the longest chain has 31 concepts.
5. **Taxonomy.** 15 categories. The largest is Microscope Instrumentation at 9.2% and the
   smallest is Fluorescence Fundamentals at 4.9%.
6. **JSON.** `learning-graph.json` has 510 nodes, 842 edges and 15 groups, and it
   passes schema validation. The top concepts by CIS are Vector Calculus, Maxwell's Equations, Electromagnetic Wave Equation, Complex Number, Complex Exponential, Phasor Notation.
7. **Pages.** Wrote `concept-list.md`, `concept-taxonomy.md`, `index.md`, and
   added the learning-graph pages to the `nav:` in `mkdocs.yml`.
