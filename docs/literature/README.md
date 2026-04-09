# Literature Directory

This directory contains research papers, references, and literature relevant to the project.

## Guidelines:
- Store research papers, articles, and reference materials
- Include both primary and secondary sources
- Organize by topic, author, or chronological order
- Maintain proper citation information
- Consider copyright and fair use policies

## File Organization:
- Use subdirectories for different research areas or topics
- Include bibliographic information (BibTeX files recommended)
- Store PDFs with descriptive filenames
- Consider using citation management tools (Zotero, Mendeley, etc.)

## Recommended Structure:
```
literature/
├── primary_sources/       # Original research papers
├── reviews/              # Review articles and meta-analyses
├── methodology/          # Papers on methods and techniques
├── references.bib        # BibTeX bibliography file
└── reading_list.md       # Curated reading list with notes
```

## Citation Management:
- Maintain a central bibliography file (references.bib)
- Use consistent citation styles
- Include DOIs and URLs when available
- Document access dates for web resources

## Available Tools:

### extract_pdf_text.py
A Python utility for extracting and analyzing text from research papers in PDF format.

**Purpose**: Extract full text from PDF files and search for specific statistical analysis details, particularly useful for literature reviews and methodology analysis.

**Features**:
- Extracts complete text from PDF files using PyPDF2
- Searches for statistical analysis patterns (t-tests, statistical terms, methodology sections)
- Identifies specific analysis approaches and contrasts
- Saves extracted text for manual inspection
- Provides occurrence counts for statistical terms

**Usage**:
```bash
python extract_pdf_text.py
```

**Requirements**:
- PyPDF2 library (`pip install PyPDF2`)
- PDF file in the same directory (currently configured for "pernet_2015.pdf")

**Output**:
- Console output with statistical analysis findings
- Full text saved as `.txt` file for manual review
- Pattern matching results for research methodology

**Use Cases**:
- Literature review and methodology extraction
- Statistical analysis comparison across papers
- Automated content analysis of research publications
- Text mining for specific research terms and approaches 