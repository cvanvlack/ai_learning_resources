# Gihub Copilot

# VS Code Keyboard Shortcuts
- `Tab` - Accept suggestions
- `Esc` - Reject suggestion
- `Ctrl + Enter` - Open Copilot (will open a separate panel showing 10 suggestions)
- `Alt/Option + ]` - Next suggestion
- `Alt/Option + [` - Previous suggestion
- `Alt/Option + \` - Trigger in-line Copilot (Coplit hasn't given a suggestion or the suggestion has been rejected and wants to manually trigger it to provide a suggestion)
- `Ctrl + →` - Partially accepting suggestions

# Visual Studio Keyboard Shortcuts
- `Tab` - Accept suggestions
- `Esc` - Reject suggestion
- `Ctrl + Enter` - Open Copilot (will open a separate panel showing 10 suggestions)
- `Alt + .` - Next suggestion
- `Alt + ,` - Previous suggestion

## Not sure about these
- `Ctrl + Alt + \` - Trigger in-line Copilot (Coplit hasn't given a suggestion or the suggestion has been rejected and wants to manually trigger it to provide a suggestion)
- `Ctrl + →` - Partially accepting suggestions

# How to get Better Suggestions
- Add a block comment at the top of the file describing what the file is for.
- Close open files that are not related to the code you are working on.
- Open files that are related to the code you are working on.
- Add imports that you know you are going to use.
- Be diligent about descriptive variable and function names.
- Be diligent about good programming practices and focus on HIGHLY READABLE code.
- Add docstrings to your functions and keep them up to date. If you update a function signature, update the docstring with /doc from copilot chat.
- Delete unused or commented code
- Copy and paste concrete examples of formats. E.g. if you have a specific datetime format, copy it into the doc for the function. Or if you are parsing a link or a .json structure, either add it to a docstring or add it in an open file in your editor.
- Don't try to get copilot to write entire blocks of code for you. The larger the chunk of code, the less likely it is to be correct. Instead, use copilot to write small chunks of code and then iterate on it.
- If variable types are optional in your programming language, add them. Copilot will be able to infer more about what you are trying to do.

# References
 - [GitHub Copilot in VS Code - Inline Suggestions](https://code.visualstudio.com/docs/editor/github-copilot#_inline-suggestions)
 - [Getting started with GitHub Copilot](https://docs.github.com/en/copilot/using-github-copilot/getting-started-with-github-copilot#partially-accepting-suggestions-1)
 - [Configuring GitHub Copilot in your environment - Visual Studio](https://docs.github.com/en/copilot/configuring-github-copilot/configuring-github-copilot-in-your-environment)
 - [Configuring GitHub Copilot in your environment - VS Code](https://docs.github.com/en/copilot/configuring-github-copilot/configuring-github-copilot-in-your-environment?tool=vscode)
