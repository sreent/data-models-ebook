# Data Models Ebook

A hands-on course textbook covering the major data-modelling paradigms — relational, document, XML, RDF/knowledge-graph, and property-graph — through a single progression of real-world case studies. Each chapter builds on the vocabulary, schemas, and scenarios introduced earlier, with cross-references back to where each concept was first developed.

**Audience:** University students or working professionals studying data modelling, database design, or knowledge engineering. Assumes basic SQL familiarity; no other prerequisites.

## Chapters at a Glance

| # | Topic | Key Technologies |
|---|-------|-----------------|
| 1 | Scenario Reasoning | Conceptual modelling |
| 2 | ERD to Schema Translation | ER diagrams, relational mapping |
| 3 | Normalisation | Functional dependencies, BCNF |
| 4 | SQL Querying | Joins, aggregation, subqueries |
| 5 | Enforcement | Constraints, triggers, transactions |
| 6 | Document Modelling | MongoDB, embedded vs. referenced |
| 7 | XML Contracts | XSD, XPath, DTD, namespaces |
| 8 | RDF and Knowledge Graphs | Turtle, ontologies, linked data |
| 9 | SPARQL Querying | SPARQL, graph pattern matching |
| 10 | Property Graphs and Cypher | Neo4j, traversal, fraud detection |
| 11 | Multi-Model Capstone | Cross-paradigm design exercise |

## Hands-on Labs

Every chapter has a companion lab exercise. Colab notebooks run in the browser — no local installation required. Markdown labs are pen-and-paper or discussion exercises.

| # | Lab | Open |
|---|-----|------|
| 1 | Scenario reasoning | [Markdown](hands-on-labs/01-lab-scenario-reasoning.md) |
| 2 | ERD to schema translation | [Markdown](hands-on-labs/02-lab-erd-to-schema.md) |
| 3 | Normalisation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/03-lab-normalisation.ipynb) |
| 4 | SQL querying | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/04-lab-sql-querying.ipynb) |
| 5 | Enforcement | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/05-lab-enforcement.ipynb) |
| 6 | Document modelling | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/06-lab-document-modelling.ipynb) |
| 7 | XML contracts | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/07-lab-xml-contracts.ipynb) |
| 8 | RDF and knowledge graphs | [Markdown](hands-on-labs/08-lab-rdf-and-knowledge-graphs.md) |
| 9 | SPARQL querying | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/09-lab-sparql-querying-knowledge-graphs.ipynb) |
| 10 | Property graphs and Cypher | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-ebook/blob/main/hands-on-labs/10-lab-property-graphs-cypher-traversal.ipynb) |
| 11 | Multi-model capstone | [Markdown](hands-on-labs/11-lab-multi-model-capstone.md) |

**Reading without the labs.** The book is self-contained — every query result and worked example is shown inline. You can read the entire book without running a single lab. The labs deepen understanding; they don't gate it.

## Repository Structure

```
data-models-ebook/
├── hands-on-labs/          Lab exercises (Colab notebooks + Markdown)
├── resources/              Seed data, schemas, and generators by domain
│   ├── orders-payments/        Chapters 2–5 (relational)
│   ├── ridelink/               Chapters 1, 6, 11 (super-app)
│   ├── e-invoicing/            Chapter 7 (XML/XSD)
│   ├── movie-kg/               Chapters 8–9 (RDF/SPARQL)
│   └── financial-transfers/    Chapter 10 (property graph)
├── LICENSE
└── README.md
```

See [`resources/README.md`](resources/README.md) for full dataset documentation, file inventories, and naming conventions.

## License

This project is licensed under the [MIT License](LICENSE).
