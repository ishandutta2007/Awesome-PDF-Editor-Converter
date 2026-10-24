# Awesome-PDF-Editor-Converter

## Top PDF Editor & Converter Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Self-Hosted Editing, Browser-Local Conversion & Offline-First Document Management*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **PDF Editor & Converter** tools. These tools handle the practical work of editing and transforming PDFs — modifying text and images, merging and splitting, converting to and from Office formats, applying OCR, and managing signatures — with a spectrum running from polished commercial suites to self-hosted and offline-first tools that keep your documents on your own machine.

**Examples** include Stirling-PDF, PDFApps, LocalPDF Studio, LibreOffice Draw, and PDF24 Creator (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, privacy-preserving local processing, and transparent file handling — ideal for teams handling contracts, invoices, or sensitive documents that shouldn't leave the building just to get converted.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **Adobe Acrobat Pro** — **The reference commercial PDF editor.** Full editing, OCR, form creation, redaction, and e-signatures. **Standard at $12.99/month or $155.88 annually**; **Pro at $19.99/month**. **Trade-offs**: resource-heavy background processes, subscription lock-in, and cloud dependency for many features. **Best for enterprises standardized on Adobe** needing the most complete editing toolchain.

- **Foxit PDF Editor** — Commercial PDF editor with fast rendering, annotation, and form tools. Free Reader available; paid Editor for full editing. **Best for Windows users** wanting Adobe compatibility without Adobe's resource footprint.

- **Nitro Pro** — Commercial PDF editor with editing, conversion, OCR, and e-sign. Perpetual and subscription licensing options. **Best for teams** wanting a perpetual-license alternative to Adobe's subscription.

## Open-Source GitHub Projects

- **Stirling-PDF** — **The most complete self-hosted PDF toolkit.** Open-core licensed, **50+ PDF operations in one Docker container**: merge, split, rotate, reorganize, compress, repair, OCR (via Tesseract), convert to/from images, Word, PowerPoint, HTML, Markdown, and CSV (via LibreOffice), add/remove passwords, watermark, certify/sign, redact, flatten, extract images, and compare two PDFs . **Stirling PDF 2.0** added native desktop apps for Windows, macOS, and Linux, text editing (alpha, paid), and a redesigned interface with undo/redo and version history . **Stirling PDF 3.1** moved group signature ("Stirling Sign") out of alpha and introduced a faster Office converter (beta) . **Privacy by architecture**: files exist only client-side, in server memory during task execution, or temporarily on disk for the task — any downloaded file is deleted from the server by that point . **Resource requirements**: 2 GB RAM minimum, 4 GB recommended . **Licensing**: free for individuals and teams up to 5 users; commercial license required for larger organizations ($99/month or $1,000/year for server deployment) . **Best for teams wanting a private, self-hosted Acrobat replacement** with the broadest tool coverage in one place.

- **PDFApps** — **The offline, subscription-free desktop PDF editor and manager.** Open-source, cross-platform on **Windows, macOS, and Linux** . **Editor features**: drag-and-drop file opening, continuous scroll with all pages visible, **signature support** (draw, type with cursive fonts, or import image; save for reuse; drag to place), undo/redo with full action history, color picker for text/highlights/redactions/drawings, **redact, insert text, images, highlights, notes, forms, and edit existing text** . **Other highlights**: **Pipeline mode** to apply multiple tools in sequence (e.g., rotate then compress) and save at the end, auto-update for direct installs, multi-language support (EN, PT, ES, FR, DE, ZH, IT, NL), recent files history, screen reader accessibility, dark/light theme, and cross-platform availability . **Installer includes automatic OCR engine (Tesseract) and Ghostscript detection and installation** . **Tech stack**: PySide6 (Qt 6), PyMuPDF for rendering, pypdf for manipulation, Tesseract for OCR, python-docx for DOCX export . **Available via Microsoft Store, winget, Snap, Flatpak, AppImage, Homebrew, and distro packages** . **Best for desktop users** wanting a complete offline PDF editor with text editing, signatures, and OCR without subscriptions or cloud dependency.

- **LocalPDF Studio** — **The 100% offline privacy-first PDF toolkit.** **AGPL-3.0 licensed**, cross-platform on Windows, macOS, and Linux . **All processing happens locally — nothing is uploaded** . **Features**: add comments, hand signatures, highlights, text, drawings, or images (powered by Mozilla PDF.js), presentation mode, merge multiple PDFs, split large PDFs, delete/reorder/crop pages, convert PDF pages to high-quality images, add page numbers or watermarks, lock/unlock PDFs with passwords, edit metadata, extract images, remove all metadata, convert images to PDF, **OCR on image or PDF**, **redact PDF content**, convert colorful PDFs to grayscale, build fillable PDF forms with text fields/checkboxes/radio buttons, and add filters or crop/resize images . **The honest limitation**: it is a toolkit, not a full text-editing word processor — for editing existing paragraph text, LibreOffice Draw or PDFApps are better fits . **Best for privacy-focused users** wanting a comprehensive offline PDF tool without cloud uploads.

- **LibreOffice Draw** — **The free desktop PDF editor bundled with LibreOffice.** **Opens foreign PDFs as graphical documents** — text and images become selectable snippets rather than continuous text . **Editing works best on simpler documents**: you can replace images, edit text line-by-line, add text boxes, annotate, sign, and manage pages (resize, rotate, delete, duplicate, add, reorder) . **Tight integration with other LibreOffice apps** lets you copy charts and diagrams directly into the PDF . **The honest limitations**: **complex layouts may require manual cleanup** — text reflow can break when replacing multiple lines; **no built-in merge or split** — you need separate tools for that; **no PDF compression or conversion to Word** . **Best for quick fixes and simple edits** where you already have LibreOffice installed, accepting that it is not a purpose-built PDF editor.

- **PDF24 Creator** — **The freeware Windows PDF suite with a virtual printer and OCR.** **Freeware (proprietary license)** — not open source, but free to use . **Windows-only**, in development since 2006, available in 32 languages . **Installs as a virtual printer** so you can create PDFs from any application . **Toolkit includes**: merge multiple PDFs, rotate/extract/insert pages, integrated preview for editing, encryption/decryption/signing, metadata editing, compression, watermarking/stamping, conversion to and from PDF, multiple virtual printers, integrated PDF reader, **Tesseract OCR engine**, and **redaction/caviardage** since version 10.0.0 . **Uses open-source components privately**: PDFBox, QPDF, and Ghostscript . **Best for Windows users** wanting a free, feature-rich PDF suite with printer-driver convenience, accepting that it is freeware rather than open source.

- **Apache PDFBox** — **The open-source Java library for PDF creation and manipulation.** Apache 2.0 licensed, with **creation of new PDFs, manipulation of existing documents, text extraction, and command-line utilities** . **Renders to Gray, RGB, or ARGB; exports and imports AcroForm data** . **Best for Java developers** embedding PDF generation or extraction into applications, not for end-user editing.

### Additional Strong Open-Source Options

- **OpenPDF** — **The LGPL/MPL Java library for PDF creation and editing.** Fork of iText 4, with **creating PDFs, manipulating existing documents, text and font support, graphics and images, tables, encryption, and page layout** . **Best for Java developers** wanting a permissively licensed library for programmatic PDF work.
- **pdf-lib** — **The JavaScript library for creating and modifying PDFs.** MIT licensed, with **add/remove/copy pages, draw text/images/vector paths, create/fill/flatten forms, embed fonts, and manage metadata** . **Best for web developers** building browser-based PDF tools.
- **PDF4QT** — **The open-source PDF editor with document comparison.** MIT licensed (relicensed from GPL), with rendering, editing, and comparison features . **Best for desktop Linux users** wanting an open-source PDF editor with comparison capabilities.

**Frameworks for building custom systems**: Combine **Stirling-PDF** for a self-hosted web UI covering 50+ operations with Docker deployment and API access, **PDFApps** for a complete offline desktop editor with text editing and signatures, **LocalPDF Studio** for privacy-first offline conversion and OCR, **LibreOffice Draw** for quick desktop edits on simple documents, and **PDF24 Creator** if you're on Windows and want a free printer-driver suite — to build a PDF editor and converter stack tailored to your need for breadth versus simplicity, web versus desktop, and privacy requirements.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- PDF editing and conversion tools differ significantly in editing depth, deployment model, and privacy posture. **Stirling-PDF processes files server-side** (though deletes them after task completion) — suitable for self-hosted infrastructure you control, not for shared hosting . **PDFApps and LocalPDF Studio work entirely offline** with no file uploads, making them the safest choice for sensitive documents . **LibreOffice Draw's editing is limited on complex PDFs** — text reflow can break, and it cannot merge or split PDFs internally . **PDF24 Creator is freeware, not open source** — it bundles open-source components but the application itself is proprietary . **Browser-based SaaS tools upload documents to their servers** — unsuitable for confidential material. **Stirling-PDF's licensing requires a commercial license for organizations over 5 users** .
- Self-hosted open-source solutions require proper resource allocation (Stirling-PDF needs 4 GB RAM for comfortable use), Docker deployment configuration for web tools, and awareness that OCR of large archives is CPU-intensive.

---

**Made for teams and individuals handling PDFs without handing them to a stranger's server.**
Let's make PDF editing and conversion more open, privacy-preserving, and offline-capable.
