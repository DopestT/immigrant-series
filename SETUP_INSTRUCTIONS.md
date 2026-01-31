# Repository Setup Instructions

This document provides instructions for completing the remaining manual tasks to finalize the immigrant-series repository.

## ✅ Completed Tasks

The following structural normalizations have been completed:

1. ✅ **Folder Normalization**
   - Renamed `eleven labs/` → `elevenlabs/`
   - No folder names contain spaces

2. ✅ **Script Folder Structure**
   - Fixed double/triple nesting at `scripts/scripts/scripts/`
   - All episode .txt files moved to `/scripts/`
   - Inner nested directories removed

3. ✅ **License File**
   - Renamed `license` → `LICENSE`
   - Content unchanged (MIT License)

4. ✅ **Gitignore Created**
   - Added `.gitignore` with `.DS_Store`, `Thumbs.db`, and `*.zip`

5. ✅ **Additional Structure Fixes**
   - `automatio/` → `automation/`
   - `scenario json` → `make_scenario.json`
   - `Index.html` → `index.html`
   - `visuals` file → `visuals/prompts.md` directory structure
   - Created individual caption files `ep01.srt` through `ep06.srt`

## 📋 Manual Tasks Required

The following tasks require manual intervention through the GitHub web interface:

### TASK 6: Enable GitHub Pages

**Steps:**
1. Navigate to repository Settings
2. Go to "Pages" section in the sidebar
3. Configure:
   - **Source**: Deploy from a branch
   - **Branch**: `main`
   - **Folder**: `/site`
4. Click "Save"
5. Verify the site builds successfully
6. Confirm URL resolves: `https://dopestt.github.io/immigrant-series/`

### TASK 7: Create v1.0 Release

**Steps:**
1. Go to repository main page
2. Click "Releases" in the right sidebar
3. Click "Create a new release"
4. Configure release:
   - **Tag**: `v1.0`
   - **Target**: `main` branch
   - **Release title**: `Initial Public Release`
   - **Description**:
     ```
     Initial public release of the immigrant-series documentary archive.
     Includes scripts, narration files, captions, visual prompts, sources, and automation workflows.
     ```
5. Click "Publish release"
6. Verify release is visible on GitHub

## ✅ Final Repository Structure

The repository now matches the expected structure:

```
immigrant-series/
├── README.md
├── LICENSE
├── .gitignore
│
├── site/
│   └── index.html
│
├── scripts/
│   ├── ep01_immigrant_definition.txt
│   ├── ep02_built_this_country.txt
│   ├── ep03_slaves_built_wealth.txt
│   ├── ep04_asians_built_infrastructure.txt
│   ├── ep05_border_crossed_them.txt
│   └── ep06_take_labor_blame_people.txt
│
├── elevenlabs/
│   └── elevenlabs_immigrant_series.csv
│
├── captions/
│   ├── ep01.srt
│   ├── ep02.srt
│   ├── ep03.srt
│   ├── ep04.srt
│   ├── ep05.srt
│   └── ep06.srt
│
├── visuals/
│   └── prompts.md
│
├── automation/
│   └── make_scenario.json
│
└── sources/
    └── sources_labor_history.md
```

## 🟢 Automation-Ready Status

The repository is now ready for:
- ✅ Make.com ingestion (via `/automation/make_scenario.json`)
- ✅ ElevenLabs batch processing (via `/elevenlabs/elevenlabs_immigrant_series.csv`)
- ✅ Public citation and media linking
- ✅ GitHub Pages deployment (pending manual configuration)
- ✅ Release tagging (pending manual creation)

---

**Note**: Once GitHub Pages and the v1.0 release are configured manually, the repository will be fully production-ready.
