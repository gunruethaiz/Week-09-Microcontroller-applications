# 🧠 Copilot Instructions for AI Coding Agents

## Project Overview
This repository focuses on ESP32 microcontroller applications, especially GPIO architecture and peripheral integration. It is structured for educational use, with clear separation between documentation, examples, and helper scripts.

## Key Directories & Files
- `main/` and `LabLED/`: Main application code and build system (CMake, ESP-IDF)
- `examples/`: Reference implementations for GPIO, ADC, and architecture deep-dives
  - `gpio-basic/`: Simple GPIO usage (e.g., `led_button_example.c`, `gpio_interrupt_example.c`)
  - `adc-samples/`: ADC sensor examples
  - `architecture-deep-dive/`: Advanced ESP32 architecture notes
- `Helper-files/`: Scripts for diagram rendering and environment setup (PowerShell)
- `image-src/` & `images/`: Source and rendered diagrams (Graphviz, PlantUML)
- Documentation: `ESP32-GPIO-Knowledge-Sheet.md`, `ESP32-GPIO-Worksheet.md`, and multiple README files

## Build & Development Workflow
- **Build System:** Uses ESP-IDF (CMake-based). Build targets are in `LabLED/`.
- **To build:**
  - Use ESP-IDF tools (`idf.py build`, `idf.py flash`) from the project root or `LabLED/`.
  - Windows users may need to run PowerShell scripts in `Helper-files/` for environment setup.
- **Debugging:**
  - Use ESP-IDF VS Code extension for integrated debugging.
  - Check `LabLED/build/` for build artifacts and logs.

## Project-Specific Conventions
- **Examples are modular:** Each example is self-contained. Copy, modify, and reference as needed.
- **Diagrams:** Source files in `image-src/` (DOT, PUML) are rendered to SVG/PNG in `images/` using helper scripts.
- **Documentation-first:** Key architectural decisions and learning objectives are documented in Markdown files at the root and in `examples/architecture-deep-dive/`.
- **Language:** Some documentation is in Thai; code and comments are in English.

## Integration Points & Dependencies
- **ESP-IDF:** Main dependency for firmware development. See [ESP-IDF Programming Guide](https://docs.espressif.com/projects/esp-idf/en/latest/).
- **VS Code Extensions:** Recommended to use Espressif's ESP-IDF extension for best experience.
- **Graphviz & PlantUML:** Used for architecture diagrams. Scripts in `Helper-files/` automate rendering.

## Quick Start for AI Agents
1. Start with `README.md` and `ESP32-GPIO-Knowledge-Sheet.md` for context.
2. Use `examples/` for reference implementations and patterns.
3. Build and flash using ESP-IDF commands; use helper scripts for diagram generation if needed.
4. Maintain modularity—new examples should follow the structure in `examples/`.
5. Update documentation when introducing new architectural concepts or workflows.

---
_Last updated: October 2025_
