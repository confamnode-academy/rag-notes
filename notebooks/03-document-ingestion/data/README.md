# Document Parsing Sample Documents

These files are intentionally different so the `02-document-parsing.ipynb` notebook
can demonstrate why document parsing is an engineering problem.

Files:
- customer_refund_policy.txt — plain text
- internal_rag_engineering_guide.md — Markdown with headings and code formatting
- support_refunds.html — HTML with navigation, metadata, headings, sections, and footer
- q3_customer_support_operating_brief.docx — DOCX with headings, paragraphs, and a table
- employee_travel_policy.pdf — PDF with headings and a table

These are synthetic but realistic training documents created for the course. They are
not copied from real organizations or confidential sources.

Suggested notebook progression:
1. Inspect the source files.
2. Parse each format with an appropriate parser.
3. Compare raw source with extracted output.
4. Identify information that was preserved, transformed, or lost.
5. Discuss what metadata/provenance should be retained.
6. Leave detailed PDF layout analysis for 03-pdf-parsing.ipynb.
