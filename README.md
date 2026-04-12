# Data Models Course

Complete course materials for learning five data models — relational, document, XML/schema validation, RDF/knowledge graphs, and property graphs — each taught through the lens of workload trade-offs. Every chapter opens with a concrete engineering failure and builds the vocabulary to prevent it.

## Course Textbook

The textbook is the primary learning resource. It covers all 11 chapters with decision frameworks, trade-off tables, and constraint mechanisms for each data model.

| Chapter | Title |
|---------|-------|
| 1 | Introduction to Data Models |
| 2 | Conceptual Modelling with ERD |
| 3 | Normalisation |
| 4 | SQL Querying |
| 5 | Enforcement |
| 6 | Document Modelling |
| 7 | XML for Contracts |
| 8 | RDF and Knowledge Graphs |
| 9 | SPARQL Querying Knowledge Graphs |
| 10 | Property Graphs and Cypher Traversal |
| 11 | Multi-Model Capstone |

**Download:** [`course-textbook/data-models-ebook.epub`](course-textbook/data-models-ebook.epub) — open with any EPUB reader ([Calibre](https://calibre-ebook.com/), [Apple Books](https://www.apple.com/apple-books/), [Thorium Reader](https://www.edrlab.org/software/thorium-reader/), or your e-reader device).

## Slides

Lecture slide decks for each chapter, located in [`slides/`](slides/):

| Chapter | Slides |
|---------|--------|
| 1 | [Introduction to Data Models](slides/Introduction%20to%20Data%20Models.pdf) |
| 2 | [Conceptual Modelling](slides/Conceptual%20Modelling.pdf) |
| 3 | [Normalisation](slides/Normalisation.pdf) |
| 4 | [SQL Querying](slides/SQL%20Querying.pdf) |
| 5 | [Enforcement](slides/Enforcement.pdf) |
| 6 | [Document Modelling](slides/Document%20Modelling.pdf) |
| 7 | [XML for Contracts](slides/XML%20for%20Contracts.pdf) |
| 8 | [RDF and Knowledge Graphs](slides/RDF%20and%20Knowledge%20Graphs.pdf) |
| 9 | [SPARQL for Graph Querying](slides/SPARQL%20for%20Graph%20Querying.pdf) |
| 10 | [Property Graphs](slides/Property%20Graphs.pdf) |
| 11 | [Multi-Model Capstone](slides/Multi-Model%20Capstone.pdf) |

## Hands-on Labs

Each lab aligns with a chapter in the textbook, using the same datasets and scenarios so you can run the queries, break the constraints, and observe the failures yourself.

Google Colab notebooks run in the browser — no local installation required. Markdown labs are pen-and-paper or discussion exercises.

| # | Lab | Technologies | Open |
|---|-----|-------------|------|
| 1 | Scenario reasoning | Conceptual modelling, scenario analysis | [Markdown](hands-on-labs/01-lab-scenario-reasoning.md) |
| 2 | ERD to schema translation | ER diagrams, relational mapping | [Markdown](hands-on-labs/02-lab-erd-to-schema.md) |
| 3 | Normalisation | SQL, functional dependencies, BCNF, star schema | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/03-lab-normalisation.ipynb) |
| 4 | SQL querying | Joins, aggregation, subqueries, window functions | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/04-lab-sql-querying.ipynb) |
| 5 | Enforcement | Constraints, triggers, transactions, ACID | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/05-lab-enforcement.ipynb) |
| 6 | Document modelling | MongoDB, embedded vs. referenced, aggregation pipeline | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/06-lab-document-modelling.ipynb) |
| 7 | XML contracts | XSD, XPath, DTD, namespaces | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/07-lab-xml-contracts.ipynb) |
| 8 | RDF and knowledge graphs | Turtle, ontologies, linked data, schema mapping | [Markdown](hands-on-labs/08-lab-rdf-and-knowledge-graphs.md) |
| 9 | SPARQL querying | SPARQL, graph pattern matching, aggregation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/09-lab-sparql-querying-knowledge-graphs.ipynb) |
| 10 | Property graphs and Cypher | Neo4j, traversal, fraud detection | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sreent/data-models-course/blob/main/hands-on-labs/10-lab-property-graphs-cypher-traversal.ipynb) |
| 11 | Multi-model capstone | Cross-paradigm architecture design | [Markdown](hands-on-labs/11-lab-multi-model-capstone.md) |

## Datasets

Each lab draws from a shared set of domain datasets kept in [`resources/`](resources/):

| Domain | Labs | What's inside |
|--------|------|---------------|
| [Orders and Payments](resources/orders-payments/) | 2 -- 5 | DDL, seed data, large performance dataset (100K+ rows), schema docs |
| [RideLink Super-App](resources/ridelink/) | 1, 6, 11 | MongoDB inserts, embedded vs. referenced designs, capstone scenario |
| [E-Invoicing (Peppol)](resources/e-invoicing/) | 7 | XSD schema, valid/invalid invoices, DTD, namespaced XML |
| [Movie Knowledge Graph](resources/movie-kg/) | 8 -- 9 | Turtle ontology, two mergeable RDF sources (103 triples) |
| [Financial Transfers](resources/financial-transfers/) | 10 | 60 accounts, 150 transfers, fraud rings in Cypher |

See [`resources/README.md`](resources/README.md) for full file inventories, naming conventions, and generator scripts.

## Repository Structure

```
data-models-course/
├── course-textbook/        The course textbook (EPUB)
├── slides/                 Lecture slide decks (PDF, one per chapter)
├── hands-on-labs/          Lab exercises (Colab notebooks + Markdown)
├── resources/              Seed data, schemas, and generators by domain
│   ├── orders-payments/        Labs 2–5 (relational)
│   ├── ridelink/               Labs 1, 6, 11 (document / capstone)
│   ├── e-invoicing/            Lab 7 (XML/XSD)
│   ├── movie-kg/               Labs 8–9 (RDF/SPARQL)
│   └── financial-transfers/    Lab 10 (property graph)
├── LICENSE
└── README.md
```

## License

This project is licensed under the [MIT License](LICENSE).
