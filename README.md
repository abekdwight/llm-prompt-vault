# LLM Prompt Vault

A repository for storing and managing LLM prompts for various tasks.

## Overview

This repository serves as a centralized collection of prompts for different Large Language Models (LLMs). It is organized to efficiently manage both model-specific prompts and task-oriented prompts that can be used across multiple LLM platforms.

## Repository Structure

```
llm-prompt-vault/
├── models/              // Model-specific prompts
│   ├── claude/
│   │   ├── system-prompts/  // System prompts for Claude
│   │   └── templates/       // Claude-specific templates
│   ├── gemini/
│   │   ├── system-prompts/  // System prompts for Gemini
│   │   └── templates/       // Gemini-specific templates
│   ├── chatgpt/
│   │   ├── system-prompts/  // System prompts for ChatGPT
│   │   └── templates/       // ChatGPT-specific templates
│   └── cline/
│       ├── custom-instructions/ // Custom instructions for Cline
│       └── templates/           // Cline-specific templates
│
└── tasks/               // Task-specific prompts (usable across models)
    ├── writing/         // Content writing prompts
    ├── coding/          // Programming assistance prompts
    ├── data-analysis/   // Data analysis prompts
    ├── translation/     // Translation prompts
    ├── prompt-engineering/ // Prompt engineering prompts
    └── summarization/   // Summarization prompts


```

## Usage Guidelines

### Model-Specific Prompts

The `models` directory contains prompts that are optimized for specific LLM platforms:

- **system-prompts**: Contains prompts that define the basic behavior and capabilities of the model
- **templates**: Contains model-specific templates optimized for that particular LLM
- **custom-instructions** (Cline only): Contains custom instructions for the Cline VSCode extension

### Task-Specific Prompts

The `tasks` directory organizes prompts by their intended use case, regardless of which LLM they are used with:

- **writing**: Prompts for creative writing, content creation, etc.
- **coding**: Prompts for programming assistance and code generation
- **data-analysis**: Prompts for analyzing and interpreting data
- **translation**: Prompts for translating content between languages
- **summarization**: Prompts for summarizing content

## Contributing

To add a new prompt:

1. Identify whether it's model-specific or task-specific
2. Place it in the appropriate directory
3. Use clear, descriptive filenames (e.g., `code-review-prompt.md`, `creative-story-generator.md`)
4. Include comments within the prompt file explaining its purpose and any specific instructions

## Supported LLM Platforms

- [Claude](https://www.anthropic.com/claude) by Anthropic
- [Gemini](https://gemini.google.com/) by Google
- [ChatGPT](https://chat.openai.com/) by OpenAI
- [Roo Code (prev. Roo Cline)](https://roocode.com/) (VSCode extension)

## License

[MIT License](LICENSE)
