# Interactive Graph Color Picker - ScottPlot Recreation

## Project Summary

This is an interactive web-based tool designed as a visual aid for developers working with ScottPlot (a popular .NET plotting library). 

Key aspects:
- **Visual Fidelity**: Mimics ScottPlot's rendering with backgrounds, axes, ticks, labels, grids, and plottables (e.g., signals and lines).
- **Customization**: Supports predefined themes (e.g., Light, Dark, Blue), ScottPlot palettes (e.g., Category10, Nord), custom theme saving/loading via localStorage, and fine-tuned manual color pickers.
- **Performance**: Handles dense plots (up to 20k points) with cached data generation for smooth interactions.
- **Export**: Outputs formatted C# code for themes/palettes (using palette classes where possible) or direct color assignments.
- **Tech Stack**: Pure HTML5 Canvas + JavaScript (no external dependencies), making it lightweight and embeddable.

Built iteratively through conversations, this tool streamlines theme prototyping for ScottPlot users, reducing trial-and-error in code.

## Features
- **Theme Management**: Select from predefined themes, ScottPlot palettes, or saved customs. Save new themes with custom names.
- **Interactive Plot**: Real-time rendering of a sample chirp waveform with trend line, intro/end markers, and adjustable point density (500–20k points).
- **Color Controls**: Manual hex color inputs for all elements (backgrounds, labels, ticks, lines, grids).
- **Code Generation**: Exports C# snippets tailored to the current setup, including palette instantiation or direct color sets.
- **Persistence**: Custom themes stored in browser localStorage.
- **Extras**: Plot control name customization (e.g., `formsPlot1` → `myPlot`), theme previews, and example data loading.

## Screenshots 
<img width="1137" height="1279" alt="Screenshot 2025-10-26 at 15 57 34" src="https://github.com/user-attachments/assets/943f5002-362c-46c0-8848-33e9f5956624" />


## How to Use
1. **Open the App**: Save the `index.html` file and open it in a modern browser (Chrome/Firefox recommended).
2. **Select a Theme**: Use the dropdown to pick predefined, custom, or palette options. The preview updates automatically.
3. **Customize**: Tweak colors via inputs or adjust plot density. The canvas redraws live.
4. **Save Custom**: Enter a name and click "Save Current as Custom Theme" – persists across sessions.
5. **Generate Code**: Copy the C# from the textarea below the plot. Paste into your ScottPlot project.
6. **Load Data**: Click "Load Example Data" for a fresh waveform if needed.

For development: Edit `index.html` directly (all logic is inline JS). No build step required.

## Installation / Deployment
- **Local**: Just open `index.html` in a browser.
- **GitHub Pages**: Upload to a repo and enable Pages for instant hosting.
- **No Dependencies**: Runs standalone; no Node.js or servers needed.

## Limitations
- Canvas-based simulation – not a full ScottPlot clone (e.g., no zooming/panning).
- Custom themes are browser-local only.
- Code assumes ScottPlot 5.x syntax; verify in your project.

## Contributing
Fork, tweak themes/palettes, or enhance the plot (e.g., add more plottables). Pull requests welcome!

## License
MIT License – feel free to use/modify/share.

---

*Built (mostly with AI - yeah, I'm not afraid to admit it). It uses HTML/JS for ScottPlot enthusiasts. Questions? Open an issue.*
