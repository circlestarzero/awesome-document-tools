# Awesome Document Tools

> A curated list of document parsing, OCR, conversion, generation, editing, rendering, and AI/Agent-ready document tools.

**Goal:** Build a practical and high-quality collection of open-source and commercial tools for working with documents across Office, PDF, scanned documents, images, CAD/BIM, and other structured formats.

## Contents

- [Document Intelligence & Unified Parsing](#document-intelligence--unified-parsing)
- [OCR & Document AI](#ocr--document-ai)
- [PDF](#pdf)
- [Microsoft Office & OOXML](#microsoft-office--ooxml)
- [Document Conversion](#document-conversion)
- [Document Generation & Templating](#document-generation--templating)
- [Spreadsheet](#spreadsheet)
- [Presentation](#presentation)
- [HTML / Markdown / EPUB](#html--markdown--epub)
- [CAD / Engineering Drawings](#cad--engineering-drawings)
- [3D CAD / Geometry](#3d-cad--geometry)
- [BIM / IFC](#bim--ifc)
- [Document Rendering & Preview](#document-rendering--preview)
- [Document Search & RAG](#document-search--rag)
- [Agent / MCP Document Tools](#agent--mcp-document-tools)
- [Cloud / Commercial APIs](#cloud--commercial-apis)
- [Libraries & SDKs by Language](#libraries--sdks-by-language)
- [Document Quality Evaluation](#document-quality-evaluation)
- [Contributing](#contributing)

---

## Document Intelligence & Unified Parsing

Tools that parse multiple document formats and preserve structure, layout, tables, figures, and metadata.

| Project | Description | Formats | License |
|---|---|---|---|
| [Docling](https://github.com/docling-project/docling) | IBM-backed document conversion and understanding toolkit with a unified document model | PDF, DOCX, PPTX, XLSX, HTML, images, etc. | MIT |
| [MinerU](https://github.com/opendatalab/MinerU) | High-quality document parsing, especially strong for PDFs, Chinese documents, tables, and formulas | PDF, DOCX, PPTX, XLSX, images | Apache-2.0 + additional terms |
| [Marker](https://github.com/datalab-to/marker) | Fast PDF/document → Markdown/JSON/HTML parser with layout, tables, formulas and OCR support | PDF, images, Office, EPUB, HTML | See project/model licenses |
| [Unstructured](https://github.com/Unstructured-IO/unstructured) | General-purpose document ingestion and partitioning framework | PDF, Office, HTML, images, email, etc. | Apache-2.0 |
| [Apache Tika](https://github.com/apache/tika) | General-purpose content detection and metadata/text extraction toolkit | Hundreds of formats | Apache-2.0 |
| [GROBID](https://github.com/kermitt2/grobid) | Machine-learning library for extracting structured scholarly documents | PDF / academic papers | Apache-2.0 |
| [LayoutParser](https://github.com/Layout-Parser/layout-parser) | Deep-learning toolkit for document image layout analysis | Images / PDFs | Apache-2.0 |

### Selection notes

- **Docling** — strong default for an Agent-oriented unified document representation.
- **MinerU** — especially worth evaluating for Chinese PDFs, complex layouts, tables, and formulas.
- **Marker** — strong PDF-to-Markdown/structured-output option.
- **Unstructured** — useful for ingestion pipelines and RAG systems.
- **Tika** — excellent as a format detector / metadata / basic extraction layer rather than a complete AI document parser.

---

## OCR & Document AI

### Open Source

| Project | Description | Strengths | License |
|---|---|---|---|
| [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR) | Full OCR and document AI toolkit | Multilingual OCR, layout, tables, formulas, document understanding | Apache-2.0 |
| [Tesseract](https://github.com/tesseract-ocr/tesseract) | Mature classical OCR engine | Broad language support, CPU, mature ecosystem | Apache-2.0 |
| [EasyOCR](https://github.com/JaidedAI/EasyOCR) | Easy-to-use multilingual OCR | Simple API, many languages | Apache-2.0 |
| [Surya](https://github.com/datalab-to/surya) | OCR and document layout models | Text recognition, layout, reading order | See project license |
| [OCRmyPDF](https://github.com/ocrmypdf/OCRmyPDF) | Adds an OCR text layer to scanned PDFs | Searchable PDF, PDF/A workflows | MPL-2.0 |
| [docTR](https://github.com/mindee/doctr) | Deep-learning OCR library | Text detection + recognition | Apache-2.0 |
| [keras-ocr](https://github.com/faustomorales/keras-ocr) | OCR pipeline built around Keras | Research/prototyping | MIT |

### Commercial / API

- [Azure AI Document Intelligence](https://azure.microsoft.com/products/ai-services/ai-document-intelligence)
- [Google Cloud Document AI](https://cloud.google.com/document-ai)
- [Amazon Textract](https://aws.amazon.com/textract/)
- [Adobe PDF Extract API](https://developer.adobe.com/document-services/docs/overview/pdf-extract-api/)
- [Mistral OCR](https://docs.mistral.ai/capabilities/document-ai/)
- [Google Cloud Vision](https://cloud.google.com/vision)
- [Azure AI Vision](https://azure.microsoft.com/products/ai-services/ai-vision)

---

## PDF

### Parsing / Extraction

| Project | Description | License |
|---|---|---|
| [PyMuPDF](https://github.com/pymupdf/PyMuPDF) | Python bindings for MuPDF; fast PDF parsing/rendering/manipulation | AGPL-3.0 / commercial |
| [Apache PDFBox](https://github.com/apache/pdfbox) | Java PDF creation, parsing, extraction and manipulation | Apache-2.0 |
| [MuPDF](https://github.com/ArtifexSoftware/mupdf) | High-performance PDF/XPS/ebook engine | AGPL-3.0 / commercial |
| [PDF.js](https://github.com/mozilla/pdf.js) | JavaScript PDF renderer/viewer | Apache-2.0 |
| [qpdf](https://github.com/qpdf/qpdf) | Low-level PDF transformation and inspection | Apache-2.0 |
| [pypdf](https://github.com/py-pdf/pypdf) | Pure Python PDF manipulation library | BSD-3-Clause |
| [pdfplumber](https://github.com/jsvine/pdfplumber) | PDF text/table extraction focused on programmatic analysis | MIT |

### OCR / Scanned PDF

- [OCRmyPDF](https://github.com/ocrmypdf/OCRmyPDF)
- [PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)
- [Tesseract](https://github.com/tesseract-ocr/tesseract)
- [Docling](https://github.com/docling-project/docling)
- [MinerU](https://github.com/opendatalab/MinerU)

### PDF Creation / Generation

- [ReportLab](https://github.com/Distrotech/reportlab) — Python PDF generation
- [WeasyPrint](https://github.com/Kozea/WeasyPrint) — HTML/CSS → PDF
- [Typst](https://github.com/typst/typst) — modern typesetting system
- [LaTeX](https://www.latex-project.org/) — scientific/technical document generation
- [Prawn](https://github.com/prawnpdf/prawn) — Ruby PDF generation

---

## Microsoft Office & OOXML

### DOCX

- [python-docx](https://github.com/python-openxml/python-docx) — create/read/modify DOCX
- [docxcompose](https://github.com/4teamwork/docxcompose) — concatenate and compose DOCX
- [docxtpl](https://github.com/JessicaTegner/docxtpl) — Jinja2-based DOCX templating
- [Mammoth](https://github.com/mwilliamson/mammoth.js) — DOCX → HTML conversion

### XLSX

- [openpyxl](https://github.com/ericgazoni/openpyxl) — read/write XLSX
- [XlsxWriter](https://github.com/jmcnamara/XlsxWriter) — generate XLSX with formatting/charts
- [SheetJS](https://github.com/SheetJS/sheetjs) — JavaScript spreadsheet parser/writer
- [ExcelJS](https://github.com/exceljs/exceljs) — JavaScript XLSX library
- [DuckDB](https://github.com/duckdb/duckdb) — useful for analytical spreadsheet/data workflows

### PPTX

- [python-pptx](https://github.com/scanny/python-pptx) — create/read/modify PPTX
- [PptxGenJS](https://github.com/gitbrent/PptxGenJS) — JavaScript PowerPoint generation

### Office-compatible editors

- [LibreOffice](https://github.com/LibreOffice/core) — full office suite and headless conversion
- [ONLYOFFICE Docs](https://github.com/ONLYOFFICE/DocumentServer) — web-based Office editor/server
- [Collabora Online](https://github.com/CollaboraOnline/online) — browser-based LibreOffice-derived office suite

---

## Document Conversion

| Tool | Typical Use | License |
|---|---|---|
| [Pandoc](https://github.com/jgm/pandoc) | Markdown/HTML/LaTeX/Office/EPUB and many other conversions | GPL-2.0 |
| [LibreOffice](https://github.com/LibreOffice/core) | Office ↔ PDF and broad Office-format conversion | MPL/LGPL/GPL components |
| [Calibre](https://github.com/kovidgoyal/calibre) | EPUB/ebook conversion and management | GPL-3.0 |
| [ImageMagick](https://github.com/ImageMagick/ImageMagick) | Image format conversion and preprocessing | Apache-2.0 |
| [FFmpeg](https://github.com/FFmpeg/FFmpeg) | Multimedia conversion; useful for embedded media workflows | LGPL/GPL depending on build |

Typical pipeline:

```text
DOCX / XLSX / PPTX
        │
        ▼
   LibreOffice
        │
        ▼
       PDF
        │
        ▼
Docling / MinerU / OCR
        │
        ▼
  Document IR
```

---

## Document Generation & Templating

### General

- [Jinja2](https://github.com/pallets/jinja) — general-purpose templating
- [docxtpl](https://github.com/JessicaTegner/docxtpl) — DOCX + Jinja2 templates
- [Pandoc](https://github.com/jgm/pandoc) — structured document generation/conversion
- [Typst](https://github.com/typst/typst) — programmable typesetting
- [LaTeX](https://www.latex-project.org/) — technical/scientific document generation
- [Quarto](https://github.com/quarto-dev/quarto-cli) — reproducible scientific/technical publishing

### Agent-oriented generation pattern

```text
Agent
  │
  ▼
Structured Document Model
  │
  ├── DOCX → python-docx / docxtpl
  ├── XLSX → openpyxl / XlsxWriter
  ├── PPTX → python-pptx / PptxGenJS
  ├── HTML → template engine
  └── PDF  → Typst / WeasyPrint / LibreOffice
```

---

## Spreadsheet

### Libraries

- [openpyxl](https://github.com/ericgazoni/openpyxl)
- [XlsxWriter](https://github.com/jmcnamara/XlsxWriter)
- [SheetJS](https://github.com/SheetJS/sheetjs)
- [ExcelJS](https://github.com/exceljs/exceljs)
- [Apache POI](https://github.com/apache/poi)
- [ClosedXML](https://github.com/ClosedXML/ClosedXML)
- [EPPlus](https://github.com/EPPlusSoftware/EPPlus)

### Spreadsheet AI / Data Analysis

- [DuckDB](https://github.com/duckdb/duckdb)
- [Polars](https://github.com/pola-rs/polars)
- [Pandas](https://github.com/pandas-dev/pandas)

---

## Presentation

- [python-pptx](https://github.com/scanny/python-pptx)
- [PptxGenJS](https://github.com/gitbrent/PptxGenJS)
- [Marp](https://github.com/marp-team/marp)
- [reveal.js](https://github.com/hakimel/reveal.js)
- [Quarto](https://github.com/quarto-dev/quarto-cli)
- [LibreOffice Impress](https://github.com/LibreOffice/core)

---

## HTML / Markdown / EPUB

### Markdown

- [cmark](https://github.com/commonmark/cmark)
- [markdown-it](https://github.com/markdown-it/markdown-it)
- [mistune](https://github.com/lepture/mistune)
- [Python-Markdown](https://github.com/Python-Markdown/markdown)

### HTML → PDF

- [WeasyPrint](https://github.com/Kozea/WeasyPrint)
- [Playwright](https://github.com/microsoft/playwright)
- [Chromium](https://www.chromium.org/)
- [wkhtmltopdf](https://github.com/wkhtmltopdf/wkhtmltopdf)

### EPUB

- [Calibre](https://github.com/kovidgoyal/calibre)
- [EbookLib](https://github.com/aerkalov/ebooklib)

---

## CAD / Engineering Drawings

### DXF

- [ezdxf](https://github.com/mozman/ezdxf) — Python DXF reader/writer/manipulation
- [LibreCAD](https://github.com/LibreCAD/LibreCAD) — open-source 2D CAD application

### DWG

- [LibreDWG](https://github.com/LibreDWG/libredwg) — GNU DWG/DXF library
- [ODA Drawings SDK](https://www.opendesign.com/products/drawings) — commercial high-compatibility DWG/DGN SDK
- [Autodesk Platform Services](https://aps.autodesk.com/) — Autodesk cloud APIs

### CAD Agent Ideas

```text
CAD File
   │
   ├── Entity extraction
   ├── Layer analysis
   ├── Block/reference analysis
   ├── Dimension extraction
   ├── Text extraction
   ├── Geometry extraction
   └── Rendering
          │
          ▼
       CAD IR
          │
          ▼
        Agent
```

---

## 3D CAD / Geometry

| Project | Description | License |
|---|---|---|
| [Open CASCADE Technology](https://github.com/Open-Cascade-SAS/OCCT) | Industrial-grade open-source geometric modeling kernel | LGPL-2.1 with exception |
| [FreeCAD](https://github.com/FreeCAD/FreeCAD) | Parametric 3D CAD application with Python API | LGPL-2.1 |
| [Open3D](https://github.com/isl-org/Open3D) | 3D data processing, geometry, point clouds and visualization | MIT |
| [Assimp](https://github.com/assimp/assimp) | 3D model import/export library | BSD-3-Clause |
| [Blender](https://github.com/blender/blender) | Full 3D content creation and geometry automation | GPL-3.0 |

Common formats:

```text
STEP
IGES
BREP
STL
OBJ
PLY
3MF
GLTF / GLB
```

---

## BIM / IFC

- [IfcOpenShell](https://github.com/IfcOpenShell/IfcOpenShell) — IFC toolkit and geometry processing
- [Bonsai](https://github.com/IfcOpenShell/IfcOpenShell) — Blender-based BIM authoring environment
- [FreeCAD](https://github.com/FreeCAD/FreeCAD) — general CAD/BIM workflows
- [Open BIM / IFC.js](https://github.com/ThatOpen/engine_web-ifc) — IFC parsing in web environments

Typical Agent workflow:

```text
IFC
 │
 ▼
IfcOpenShell
 │
 ├── Elements
 ├── Properties
 ├── Relationships
 ├── Quantities
 └── Geometry
        │
        ▼
     BIM IR
        │
        ▼
      Agent
```

---

## Document Rendering & Preview

### PDF

- [PDF.js](https://github.com/mozilla/pdf.js)
- [MuPDF](https://github.com/ArtifexSoftware/mupdf)
- [PDFium](https://pdfium.googlesource.com/pdfium/)
- [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

### Office

- [LibreOffice](https://github.com/LibreOffice/core)
- [ONLYOFFICE Docs](https://github.com/ONLYOFFICE/DocumentServer)
- [Collabora Online](https://github.com/CollaboraOnline/online)

### Web / Browser

- [Playwright](https://github.com/microsoft/playwright)
- [Chromium](https://www.chromium.org/)

---

## Document Search & RAG

Document parsing should preserve structure instead of flattening everything into plain text.

### Useful components

- [LlamaIndex](https://github.com/run-llama/llama_index)
- [LangChain](https://github.com/langchain-ai/langchain)
- [Haystack](https://github.com/deepset-ai/haystack)
- [Unstructured](https://github.com/Unstructured-IO/unstructured)
- [Docling](https://github.com/docling-project/docling)

### Recommended representation

```text
Document
 ├── metadata
 ├── pages
 ├── sections
 ├── paragraphs
 ├── tables
 ├── figures
 ├── formulas
 ├── links
 └── source locations
       │
       ▼
   Chunking
       │
       ├── semantic chunks
       ├── table chunks
       ├── figure chunks
       └── page/region references
```

For high-quality RAG, retain:

- page number
- bounding box
- section hierarchy
- table coordinates
- source document ID
- source hash
- parser/model version
- extraction confidence

---

## Agent / MCP Document Tools

This section is intentionally curated separately from parser libraries.

A good Agent document tool should expose high-level operations such as:

```text
document.open()
document.inspect()
document.search()
document.extract()
document.get_page()
document.get_region()

document.create()
document.edit()
document.replace()
document.insert_table()
document.insert_image()

document.render()
document.convert()
document.export()

spreadsheet.read()
spreadsheet.write()
spreadsheet.calculate()

presentation.create_slide()
presentation.add_text()
presentation.add_image()

cad.list_entities()
cad.query_entities()
cad.get_geometry()
cad.modify_entity()

bim.query_elements()
bim.get_properties()
bim.get_geometry()
```

Potential projects/ecosystems to evaluate:

- [Model Context Protocol](https://github.com/modelcontextprotocol) — standard tool/resource interface for AI applications
- [MCP Servers](https://github.com/modelcontextprotocol/servers) — reference MCP servers and integrations
- Document-specific MCP servers should be evaluated for maintenance status, sandboxing, permissions, file-system access, and output fidelity.

> **Curation principle:** Prefer tools that expose structured document operations rather than only "convert file to text".

---

## Cloud / Commercial APIs

For production systems where maximum extraction accuracy is more important than self-hosting:

| Provider | Main Strength |
|---|---|
| [Azure AI Document Intelligence](https://azure.microsoft.com/products/ai-services/ai-document-intelligence) | OCR, layout, tables, forms, custom extraction |
| [Google Cloud Document AI](https://cloud.google.com/document-ai) | Document parsing, layout, classification, extraction |
| [Amazon Textract](https://aws.amazon.com/textract/) | OCR, forms, tables |
| [Adobe PDF Extract API](https://developer.adobe.com/document-services/docs/overview/pdf-extract-api/) | High-quality PDF structure extraction |
| [Mistral OCR](https://docs.mistral.ai/capabilities/document-ai/) | AI-native OCR and document understanding |
| [OpenAI](https://platform.openai.com/) | Multimodal document understanding and reasoning |
| [Anthropic](https://www.anthropic.com/) | Multimodal document understanding |
| [Autodesk Platform Services](https://aps.autodesk.com/) | CAD/BIM ecosystem |
| [Open Design Alliance](https://www.opendesign.com/) | DWG/DGN/CAD SDKs |

---

## Libraries & SDKs by Language

### Python

- Docling
- MinerU
- PaddleOCR
- PyMuPDF
- pypdf
- pdfplumber
- python-docx
- openpyxl
- XlsxWriter
- python-pptx
- ezdxf
- IfcOpenShell
- FreeCAD Python API

### Java

- Apache Tika
- Apache PDFBox
- Apache POI
- docx4j

### JavaScript / TypeScript

- PDF.js
- mammoth.js
- SheetJS
- ExcelJS
- PptxGenJS
- Playwright
- pdf-lib

### C / C++

- MuPDF
- PDFium
- Open CASCADE
- LibreDWG
- Assimp
- FreeCAD core

### Rust

Potential areas to investigate:

- PDF parsing/rendering
- Office/OOXML
- document conversion
- WASM document processing
- sandboxed document services

> Rust projects should be evaluated separately for maturity and production readiness rather than included solely because they are Rust-based.

---

## Document Quality Evaluation

Document tools should not be evaluated only by GitHub stars.

Recommended benchmark dimensions:

### Text

- character error rate (CER)
- word error rate (WER)
- text extraction completeness
- reading order accuracy

### Layout

- block detection
- heading hierarchy
- multi-column ordering
- header/footer detection
- bounding-box accuracy

### Tables

- table detection
- row/column reconstruction
- merged cells
- cell text accuracy
- nested tables

### Formula

- formula detection
- LaTeX conversion
- mathematical structure preservation

### Images / Figures

- figure detection
- caption association
- image extraction
- chart understanding

### Office

- paragraph/style preservation
- tables
- comments
- tracked changes
- hyperlinks
- headers/footers
- embedded objects
- formulas
- charts
- slide layouts

### CAD

- entity completeness
- layer preservation
- block/reference preservation
- geometry accuracy
- dimension extraction
- text extraction
- rendering fidelity

### BIM

- schema compatibility
- entity completeness
- properties
- relationships
- geometry
- quantities

---

## Recommended Architecture

A robust Agent Document Runtime can be built as:

```text
                         Agent
                           │
                    Document Tool API
                           │
                  ┌────────▼────────┐
                  │ Document Router │
                  └────────┬────────┘
                           │
        ┌──────────────────┼───────────────────┐
        │                  │                   │
      Office              PDF                CAD/BIM
        │                  │                   │
   OOXML Parser       Docling/MinerU       ezdxf/OCCT
        │              PaddleOCR           FreeCAD/IFC
        │                  │                   │
        └──────────────────┼───────────────────┘
                           │
                    Unified Document IR
                           │
              ┌────────────┼────────────┐
              │            │            │
             RAG          Edit        Generate
              │            │            │
           Search       Patch/AST     Office/PDF
                           │
                       Validation
                           │
                       Rendering
                           │
                       Visual QA
```

### Important design principle

**Do not make OCR or Markdown the universal intermediate representation.**

Use a structured Document IR that can retain:

```text
text
layout
geometry
tables
images
formulas
styles
relationships
source locations
confidence
```

---

## Curation Criteria

A project should preferably satisfy several of these criteria:

- Active development
- Meaningful user/community adoption
- Clear documentation
- Reproducible installation
- Production usage or credible engineering maturity
- Good format coverage
- High extraction fidelity
- Structured output
- Agent/API friendliness
- Clear license
- Commercial-use compatibility
- Security/sandboxing considerations

### Project status labels

Use these labels when expanding the list:

- `⭐ Recommended`
- `🔥 Active`
- `🧪 Experimental`
- `🏢 Commercial`
- `🔓 Open Source`
- `⚠️ License Review`
- `🖥️ GPU`
- `🌐 API`
- `🤖 Agent Ready`

---

## Contributing

Contributions are welcome.

Please submit tools that are:

1. Relevant to document processing, generation, editing, rendering, OCR, CAD/BIM, or document AI.
2. Actively maintained or historically significant.
3. Clearly documented.
4. Properly licensed.
5. Useful to developers building document automation or AI/Agent systems.

For each project, please provide:

```text
Name
URL
Category
Short description
Supported formats
License
Language
Agent/API support
Maintenance/activity
Notable strengths
Known limitations
```

Please avoid duplicate projects, abandoned wrappers, and projects whose primary purpose is unrelated to document processing.

---

## License

This curated list is released under the [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/), unless otherwise stated.
