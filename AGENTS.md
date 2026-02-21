# Prompt Engineering for AI Music Generation

## Project Overview

This project is a collection of interactive HTML-based infographics and visual guides focused on **prompt engineering techniques for AI music generation systems**. The content provides structured methodologies, formulas, and best practices for crafting effective prompts that guide AI models to generate music with specific stylistic, emotional, and structural characteristics.

The project targets users working with AI music generation tools (such as Suno, Udio, or similar platforms) who want to improve their prompt craft to achieve more predictable and higher-quality musical outputs.

## Project Structure

```
/home/mya/Documents/kimi/
├── AGENTS.md                           # This file
├── promptEngineer.code-workspace       # VS Code workspace configuration
├── meta.html                           # Specification Spectrum Diagnostic (Python-generated HTML)
├── infographic_1_signal_flow.html      # Dual-Prompt Architecture: Signal Flow
├── infographic_2_blueprint.html        # Dual-Prompt Architecture: Style vs Lyrics Blueprint
├── infographic_3_gmiv_formula.html     # The GMIV Formula (Genre + Mood + Instrumentation + Vocals)
├── infographic_4_hierarchy_dashboard.html  # Control Hierarchy Decision Matrix
├── infographic_5_meta_tag_command_center.html  # Meta Tag Command Center (CRT terminal UI)
├── infographic_6_meta_tag_encyclopedia.html    # Meta Tag Encyclopedia (Expandable Data Grid)
└── promptEngineering/                  # Git submodule (empty, only .git/)
    └── .git/
```

## Technology Stack

- **Pure HTML5 + CSS3**: All infographics are self-contained HTML files with embedded CSS
- **No JavaScript Frameworks**: No external dependencies or build tools required
- **No Build Process**: Files are ready to open directly in any modern web browser
- **Google Fonts**: Some infographics load fonts from Google Fonts CDN (Inter, Fira Code)
- **SVG**: Used for waveform visualizations and signal flow diagrams

## Core Concepts & Methodologies

### 1. Dual-Prompt Architecture
The project advocates for separating prompts into two domains:
- **Style Prompt**: Controls timbre, texture, space, genre, instrumentation, production
- **Lyrics Prompt**: Controls narrative arc, structural markers, constraints

### 2. GMIV Formula
A four-element formula for constructing style prompts:
- **G** = Genre (primary categorical anchor)
- **M** = Mood (compound emotional descriptors)
- **I** = Instrumentation (3-layer: source + technique + treatment)
- **V** = Vocals (gender, register, timbre, delivery, processing)

Optimal specification: **40-60 words** distributed across GMIV elements.

### 3. Control Hierarchy
Resolution rules when prompts conflict:
- **Specificity wins**: Local > Global
- **Temporal priority**: Later > Earlier
- **Inline tags** have highest priority (use sparingly)

### 4. Specification Spectrum
Three zones of prompt specification:
- **Under-specified**: Single-word tags, high output variance
- **Optimal (Goldilocks Zone)**: 40-60 words, precise targeting
- **Over-specified**: Mutually exclusive requirements, attribute collapse

## File Descriptions

| File | Description | Visual Style |
|------|-------------|--------------|
| `infographic_1_signal_flow.html` | Modular synthesizer-style visualization of dual-prompt signal flow | Dark rack-mount UI with knobs, LEDs, CV cables |
| `infographic_2_blueprint.html` | Technical blueprint comparing Style vs Lyrics domains | Engineering blueprint aesthetic with cyan grid |
| `infographic_3_gmiv_formula.html` | The four-element formula breakdown | High-contrast black background with color-coded cards |
| `infographic_4_hierarchy_dashboard.html` | Decision matrix for prompt conflict resolution | Glass-morphism dashboard with telemetry |
| `infographic_5_meta_tag_command_center.html` | Meta tag syntax and hierarchy reference | CRT terminal/phosphor green aesthetic |
| `infographic_6_meta_tag_encyclopedia.html` | Comprehensive tag reference with filtering | Data grid with expandable sections |
| `meta.html` | Specification spectrum diagnostic tool | Oscilloscope-style waveform visualization |

## How to Use

1. **Open any HTML file** directly in a web browser:
   ```bash
   # Example: open in default browser
   xdg-open infographic_3_gmiv_formula.html
   
   # Or on macOS
   open infographic_3_gmiv_formula.html
   ```

2. **No server required**: All files are static and self-contained

3. **No dependencies**: All CSS is embedded; only some files load Google Fonts from CDN

## Development Guidelines

### Code Style
- All CSS is embedded within `<style>` tags in each HTML file
- Consistent use of CSS custom properties (variables) for theming
- Responsive design with `@media` queries for mobile support
- Semantic HTML5 structure

### Visual Design Patterns
- Dark themes dominate (suitable for technical/music production contexts)
- Color coding:
  - Cyan (`#00f0ff`): Global/primary elements
  - Magenta (`#ff006e`): Override/section elements
  - Amber (`#ff9e00`): Warnings/medium complexity
  - Green (`#39ff14`): Success/optimal states
  - Red (`#ff073a`): Errors/high complexity/overrides

### File Naming Convention
- All lowercase with underscores
- Pattern: `infographic_{number}_{descriptive_name}.html`

## Testing

There are no automated tests in this project. Testing is manual:

1. Open each HTML file in multiple browsers (Chrome, Firefox, Safari)
2. Verify responsive layout at different viewport sizes
3. Check that all interactive elements (hover states, expandable sections) work correctly

## Deployment

These are static HTML files that can be deployed to any web server or static hosting:

- GitHub Pages
- Netlify
- Vercel
- Any standard web server (nginx, Apache)

Simply copy all `.html` files to the web root or a subdirectory.

## Notes for AI Agents

- This is a **documentation/visualization project**, not a software application
- No package managers (npm, pip, etc.) are used
- No compilation or build step required
- Files can be edited directly; changes are immediately visible when refreshed in browser
- The `promptEngineering/` directory is a git submodule that appears to be empty/uninitialized
