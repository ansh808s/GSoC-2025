# # Language Server Protocol for Makim’s YAML Configuration

## Final Work Report for the Google Summer of Code 2025 under Open Science Labs for the Makim LSP project

## Contributor Info

<div container>
<table>

<tr>
<td width="600px">
&#8226; Name - Ansh Arora<br />
&#8226; Organization - <a href="https://github.com/osl-incubator" target="_blank">Open Science Labs</a><br />
&#8226; Email - <a href="mailto:ansharora3839@gmail.com" target="_blank">ansharora3839@gmail.com</a><br />
&#8226; GitHub - <a href="https://github.com/ansh808s" target="_blank">ansh808s</a><br />
&#8226; Linkedin - <a href="https://www.linkedin.com/in/ansharora3839" target="_blank">Ansh Arora</a><br />
&#8226; Twitter - <a href="https://x.com/ansh3839" target="_blank">ansh3839</a><br />
</td>
</tr>
</table>
</div>

## Mentors' Info

- **Mentor:** [Ivan Ogasawara](https://github.com/xmnlab)

<br />

## Project Overview

**Makim** is a modern alternative to traditional Makefiles, using **YAML** to define tasks and workflows. Its goal is to provide developers with a simple, flexible, and readable way to define project automation pipelines.

The objective of my GSoC 2025 project was to enhance the developer experience for Makim by creating a **Language Server Protocol (LSP)** and a **VS Code extension** that would provide smart editor features for Makim configuration files.

<br />

## GSoC Project Page

- [Language Server Protocol for Makim’s YAML Configuration](https://summerofcode.withgoogle.com/programs/2025/projects/OPlaxDeq)

## GSoC Project Proposal

- [Project Proposal](https://github.com/ansh808s/GSoC-2025/blob/main/ansh-gsoc-proposal.pdf)

## Project Repository

- [makim-org/makim-lsp](https://github.com/makim-org/makim-lsp)

## GSoC Blogs

- [Language Server Protocol (LSP): How Editors Speak Code](https://opensciencelabs.org/blog/language-server-protocol-lsp-how-editors-speak-code)
- [Packaging a VS Code Extension Using pnpm and VSCE](https://opensciencelabs.org/blog/packaging-a-vs-code-extension-using-pnpm-and-vsce)

<br />

## Work Summary

During the Google Summer of Code 2025, I developed and published a **Language Server Protocol (LSP)** implementation for **Makim’s YAML configuration files**, along with a **Visual Studio Code extension** that integrates this LSP as a client.

The work included:

- **Language Server Implementation**
  - Built the core language server following the LSP specification.
  - Implemented **error diagnostics** for YAML validation and task definitions.
  - Added **auto-completion** for task names, dependencies, and commands.
  - Published the LSP as an **npm package** for easy reuse across editors.
- **VS Code Extension Development**
  - Created a VS Code extension that communicates with the LSP.
  - Integrated **diagnostics** to highlight errors inline.
  - Provided **IntelliSense-like auto-completion** inside `.makim.yaml` files.
  - Added **CodeLens buttons** to allow running tasks directly from the editor.
  - Packaged and published the extension for distribution.

This project significantly improved the developer experience for Makim users by enabling an **intuitive and interactive workflow inside the editor**, reducing the friction of working with YAML-based automation tasks.

## Challenges Faced

- **Publishing the LSP**: Ensuring the package worked seamlessly across multiple VS Code environments.
- **YAML Parsing and Validation**: Handling dynamic workflows with nested dependencies required careful design to provide accurate diagnostics and auto completions.

## Pull Requests

| Title                                                  | Link                                                  |
| ------------------------------------------------------ | ----------------------------------------------------- |
| feat: Initial repository setup                         | [#1](https://github.com/makim-org/makim-lsp/pull/1)   |
| Setup Language server and client                       | [#2](https://github.com/makim-org/makim-lsp/pull/2)   |
| feat: add makim language configuration and grammar     | [#3](https://github.com/makim-org/makim-lsp/pull/3)   |
| feat: Add error handling and diagnosis in makim files  | [#4](https://github.com/makim-org/makim-lsp/pull/4)   |
| refactor: diagnosis feature                            | [#5](https://github.com/makim-org/makim-lsp/pull/5)   |
| feat: add ci workflow and unit tests for diagnosis     | [#6](https://github.com/makim-org/makim-lsp/pull/6)   |
| fix: match pnpm version with package.json              | [#7](https://github.com/makim-org/makim-lsp/pull/7)   |
| feat: auto completion functionality in language server | [#8](https://github.com/makim-org/makim-lsp/pull/8)   |
| feat: add code lens button to run makim tasks          | [#10](https://github.com/makim-org/makim-lsp/pull/10) |
| chore: package vscode extension                        | [#11](https://github.com/makim-org/makim-lsp/pull/11) |
| chore package language server                          | [#12](https://github.com/makim-org/makim-lsp/pull/12) |
| chore: add executable file                             | [#13](https://github.com/makim-org/makim-lsp/pull/13) |
| fix: change package manager to npm                     | [#14](https://github.com/makim-org/makim-lsp/pull/14) |
| chore: remove packaged extension                       | [#15](https://github.com/makim-org/makim-lsp/pull/15) |
| chore: add license, readme and pre publish script      | [#16](https://github.com/makim-org/makim-lsp/pull/16) |
| chore: add extension icon                              | [#17](https://github.com/makim-org/makim-lsp/pull/17) |

Code can be found [here](https://github.com/makim-org/makim-lsp/pulls?q=is%3Apr+is%3Aclosed+author%3Aansh808s).

## Future Work

- **Support for other editors**: Extend LSP integration to Neovim, Sublime Text, and other LSP-compatible editors.
- **Advanced IntelliSense features**: Task suggestions based on project context.

## Acknowledgment

I am very thankful to my mentor [Ivan Ogasawara](https://github.com/xmnlab). Without them, the work never would have been this joyful and rewarding. I love the Open Science Labs community for its welcoming and enthusiastic nature. They have been very supportive and understanding and are always open to newer ideas. Final thanks to Google for organizing this fantastic program. I feel GSoC made it easier for me to get started with open-source contributions. It was a great lesson on building and maintaining projects with great quality. I am excited to continue contributing to the open-source community.
