# Computer Security Lecture Summary

Comprehensive LaTeX-based lecture summary for a university-level
Computer Security course covering cryptography, authentication,
network security, web security, and systems security.

> Language: German 🇩🇪

The project focuses on structured technical documentation,
formal security concepts, and concise explanations of attacks,
protocols, and cryptographic constructions.

---

## Topics Covered

- Symmetric Cryptography
- Asymmetric Cryptography
- IND-CPA / IND-CCA Security
- One-Time Pad
- DES, Triple DES, AES
- Modes of Operation (ECB, CBC, CTR)
- Padding Oracle Attacks
- Hash Functions
- MACs & HMAC
- Authenticated Encryption
- Network Security
- Authentication & Authorization
- Web Security Concepts
- Security Models & Threat Analysis

---

## Build Instructions

Requirements:
- A LaTeX installation (e.g. MikTeX or TeX Live)
- Installation of the [TU Template](https://github.com/tudace/tuda_latex_templates) and the required plugins
- Installation of Pygments (for code blocks), e.g. via `pip install Pygments`

First, the folder structure must of course be downloaded, for example using `git clone`.  
Afterwards, the summary/document must be compiled with the `--shell-escape` flag.  

If you are using VS Code with LaTeX Workshop, you can modify the `settings.json` by appending the following:

```jsonc
"latex-workshop.latex.tools": [
    {
        "name": "latexmk",
        "command": "latexmk",
        "args": [
            "--shell-escape",
            "-synctex=1",
            "-interaction=nonstopmode",
            "-file-line-error",
            "-lualatex", // alternatively: "-pdf", etc.
            "-outdir=%OUTDIR%",
            "%DOC%"
        ]
    },
],
```

---

## Preview

The compiled PDF can be found in:

```text
output/summary.pdf
```

---

## Goals of the Project

- Create a structured and maintainable security reference
- Summarize theoretical and practical security concepts
- Provide concise explanations of modern cryptographic mechanisms
- Improve technical documentation and LaTeX workflow skills

---

## Disclaimer

This document was independently written for educational purposes.
It is intended as a personal lecture summary and study reference.

Some topics may be based on university lecture material and publicly
known security concepts. All rights to original course content remain
with their respective owners.

---

## License

This repository is licensed under the MIT License.
