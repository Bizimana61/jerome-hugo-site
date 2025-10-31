
---
title: "Cursor IDE Redesign — HCI Project"
date: 2025-10-30T12:00:00
draft: false
---

# Cursor IDE Redesign — HCI Project

Project overview

This project represents a comprehensive redesign of the Cursor IDE, developed as part of an HCI (Human-Computer Interaction) class. Through rigorous needfinding, prototyping, and user testing methodologies, we identified and addressed critical usability gaps that hinder Cursor's potential as an AI peer-programmer tool.

Repository: https://github.com/Bizimana61/Cursor-Redesign

## Research objectives

Our research focused on improving three core areas:

- **AI collaboration** — enhancing the interaction between developers and AI assistants
- **Version control** — streamlining git workflows and commit management
- **Workflow efficiency** — optimizing the developer experience for productivity

## Design process

1. **Needfinding**

	 Through user interviews, surveys, and observational studies, we identified key pain points in the current Cursor IDE experience:

	 - Unclear AI suggestion workflows
	 - Inefficient file management systems
	 - Poor integration of version control features
	 - Lack of contextual code assistance

2. **Prototyping**

	 We developed a fully functional prototype that addresses these issues through:

	 - Intelligent Code Suggestions: Context-aware algorithm recommendations (linear → binary search optimization)
	 - Streamlined UI: Clean, Fluent UI-based interface with improved navigation
	 - Enhanced File Management: Dynamic file creation and organization
	 - Integrated Version Control: Simplified commit workflows with visual history

3. **User testing**

	 The prototype underwent extensive user testing to validate design decisions and iterate on user feedback.

## Features implemented

- 🚀 **Starter Page Experience**
	- Professional onboarding with Cursor branding
	- Three primary action paths: "Open Project", "Clone Repo", "Connect via SSH"
	- Smooth transitions to main IDE environment

- 🎯 **AI-Powered Code Assistance**
	- Smart Algorithm Suggestions: Type "implement search" → Linear search algorithm
	- Optimization Detection: Type "optimize" → Automatic binary search upgrade
	- Visual Code Review: Side-by-side code and explanation panels
	- Accept/Reject Workflow: Green highlighting with clear action buttons

- 📁 **Enhanced File Management**
	- Dynamic File Creation: Files appear only after user acceptance
	- Persistent Storage: LocalStorage-based file persistence
	- Visual File Explorer: Clean sidebar with proper file icons
	- Active File Highlighting: Clear indication of current file

- 🔄 **Integrated Version Control**
	- Simplified Commits: One-click commit with custom naming
	- Visual History: Timestamp-based commit tracking
	- Hash Generation: Automatic commit hash creation
	- Persistent History: Saved across sessions

- 🎨 **Design System**
	- Fluent UI Integration: Microsoft's design system for consistency
	- Responsive Design: Works across different screen sizes
	- Accessibility: Keyboard navigation and ARIA compliance
	- Professional Aesthetics: Clean, modern interface

## Technical implementation

### Current tech (prototype)

- Frontend: HTML5, CSS3, JavaScript (ES6+)
- Design System: Microsoft Fluent UI components and design tokens
- Storage: Browser localStorage for session persistence
- Architecture: Standalone web application (no build dependencies)

### Production stack (planned)

- Backend: Django REST API, PostgreSQL, WebSocket support (Django Channels)
- AI integration: Multi-LLM architecture (OpenAI, Anthropic, Google, Meta, local models)
- Frontend (planned): React 18 + TypeScript, Redux Toolkit, Monaco Editor, Fluent UI

## Key files & entry points

- `cursor-starter-fluent.html` — prototype entry point
- `cursor-ide-fluent.html` — full IDE interface prototype

## Running the prototype

Method 1 — Local HTTP server (recommended):

```bash
cd cursor-clone
python3 -m http.server 8000
# then open http://localhost:8000/cursor-starter-fluent.html
```

Method 2 — Direct file access: open `cursor-starter-fluent.html` in your browser.

## Research insights & outcomes

- Users prefer visual code previews over text-only suggestions
- Contextual AI assistance significantly improves workflow efficiency
- Simplified version control reduces cognitive load
- Clean UI design enhances focus and productivity

## Contributors & credit

Project team:

- Chibueze Kingsley Anyachebelu — Developer & UX Researcher
- Jerome Bizimana — Developer & User Experience Designer

Developed as part of HCI coursework focusing on needfinding, prototyping, and user testing methodologies for improving developer tools and AI-assisted programming environments.
