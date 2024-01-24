# Copilot Chat
## Copilot Chat Sidebar

## Inline Copilot Chat
Inline chat is probably the feature I use most often, after the copilot ghost text/chat completions.

- Can insert code into a new file
- Can add tests
- Can tell you how to run tests
- `@workspace`
- `@vscode`
- right click on a line and select "Ask Copilot"
- The benefits of having this all in the IDE is that it prevents breaking the "flow". If you have to do a google search for the error, scroll through an ad-filled blog post, and then copy and paste the code into your IDE, you've broken the flow. 
- `/explain`
  - Really helps when jumping into a project or a set of code that you haven't worked on before to help you get your footing.
  - Great for use on regular expressions
  - Chat can create links to files that you can click on to open in your IDE
  - You can use the `#` to choose more context to intentionally send to co-pilot.
  - You can have multiple conversation threads open at once.
  - When copilot doesn't have context on something, it will specifically ask you for more context. This is especially important when it's asking for debugging information as you don't want co-pilot accidentally scraping sensitive information and sending it to Github. Hence why it asks you.
- Options added to quick fix

- Sparkly icon shows places where copilot can suggest. 
- Best one is commit messages.
- Where are all of the right click options?
- Can push the refresh button for looking at your history of chats
- Can export a chat as .json. Can be used to add the chat to version control to to share it with someone else so they can import it.
- If you hit the X button on previous chats, you can edit the prompt history to reduce the context window so you don't confuse the model.
- `Shift F9` will take you up to previous chat boxes.
- `F9` will take you down to later chat boxes.
- Using `Create Workspace` is good when you want to create a small starter project for something.
- Using `Create Notebook` is good when you want to spin up a Jupyter notebook to try something out. If you seed the prompt with what you are attempting to do, it will propose the different sections as a template, fill them in and provide a `Create Workspace` button to create a new workspace with the notebook and the code.
- If you need to use the question "Where does this exist in my code?" copilot can't send your entire codebase to the server. If you just ask the question, "Where is the login performed" it will give you a generic answer. However, if you use the `@workspace` command, it will run locally on your machine to find any potentially relevant code in your workspace and send that to copilot to help find the right answer.``
- Can potentially use `@workspace /explain` to get a better answer to a question about all the places that use a particular function.
- In Visual Studio, it looks like you can get [AI suggested renaming options](https://devblogs.microsoft.com/visualstudio/ai-powered-rename-suggestions/).
