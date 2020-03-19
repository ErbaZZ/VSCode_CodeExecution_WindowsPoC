# VSCode Python Extension Code Execution 

**Adapted to be working on Windows, original by [doyensec](https://github.com/doyensec/VSCode_PoC_Oct2019).**

This repository contains the Proof-of-Concept of a code execution vulnerability discovered in the [Visual Studio Code](https://code.visualstudio.com/) Python extension.

>TL;DR: VScode may use code from a virtualenv found in the project folders without asking the user, for things such as formatting, autocompletion, etc. This insecure design leads to arbitrary code execution by simply cloning and opening a malicious Python repository.

You can read more about this vulnerability on our blog: [https://blog.doyensec.com/2020/03/16/vscode_codeexec.html](https://blog.doyensec.com/2020/03/16/vscode_codeexec.html).

## HowTo

- Clone the 'malicious' repository with `git clone https://github.com/ErbaZZ/VSCode_CodeExecution_WindowsPoC`
- Add the cloned repo to a VSCode workspace (Working on Windows)
- Open `main.py` in VScode
