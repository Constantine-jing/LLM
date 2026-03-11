# LLM Probes — Presentation

## How to Render

### Prerequisites

1. **Install Quarto** (if you haven't already):
   - Download from: https://quarto.org/docs/get-started/
   - Or via conda: `conda install -c conda-forge quarto`

2. **Install Python dependencies** (for code blocks):
   ```bash
   pip install jupyter numpy scikit-learn transformers torch
   ```

3. **VS Code Setup** (recommended):
   - Install the **Quarto extension** for VS Code
   - Open this folder in VS Code
   - Open `llm-probes.qmd`
   - Click the "Preview" button or press `Ctrl+Shift+K`

### Render from Command Line

```bash
# Render to HTML (Reveal.js slides)
quarto render llm-probes.qmd

# Preview with live reload
quarto preview llm-probes.qmd
```

The output HTML file will be created in the same directory (or `_output/` if configured).
Open it in any browser to view the presentation.

### Presentation Controls

Once open in browser:
- **Arrow keys** or **Space**: Navigate slides
- **F**: Fullscreen
- **S**: Speaker notes view
- **O**: Overview/grid view
- **Esc**: Exit fullscreen or overview
- **?**: Show all keyboard shortcuts

## File Structure

```
llm-probes-presentation/
├── _quarto.yml          # Quarto project configuration
├── llm-probes.qmd       # Main presentation file
├── custom.scss           # Custom theme/styling
└── README.md             # This file
```

## Notes

- The code blocks in the tutorial slides have `eval: false` so they won't 
  actually run during rendering (they're for demonstration purposes).
- If you want to run the code interactively, you can do so in a Jupyter 
  notebook or Python script separately.
- The Mermaid diagrams render automatically — no extra setup needed.
- The presentation uses Reveal.js format with a custom navy/coral color scheme.
