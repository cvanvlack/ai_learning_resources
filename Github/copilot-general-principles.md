# Copilot General Principles

1. Copilot makes suggestions based on the context of the code you are writing. It gets this context from
     - The surrounding code in your file.
     - The other open files in your editor.
         - I have read that the order it reads those tabs is from inside to out.
     - The imports in your files.
     - Sample code you provide it.
     - The specific comments you have in your file.
     - If your repo is hosted on Github, it sounds like Github will also do some extra indexing of your repo that could help with suggestions.
  <!-- todo add a link to the timestamp of the video -->
2. Copilot is not a code generator. It is a code suggestion tool. It will not write your code for you. It will give you suggestions for what it thinks you might want to write next.
3. Copilot does not get it's context from every file in your project.
  
## Principles
1. One of the recommendations is to always start each file with a comment block summary that describes, at a high level, the purpose of the file. This seeds copilot with the context it needs to know where it's going to go.
2. Good function and variable names are important. Copilot will use the names of functions and variables to help it make suggestions.
This is a paragraph with an inline comment.
<!-- Todo add a link to the md about copilot chat /doc --> 
3. Adding docstrings to your functions will further improve copilot's suggestions.
4. The more open source/common libraries you are using, the more likely copilot will have a good basis for pulling suggestions for you.
5. Having a million tabs open in your editor is likely to confuse copilot. It will have a hard time knowing which tabs to use for context.
<!-- Todo add a link to the md about copilot chat and how to import code into the chat -->
<!-- Todo eventually link to chatGPT docs -->  
6. Copilot is REALLY good and taking templated code and acting like autocomplete on steriods and helping you generate more code like that. But this is a double-edged sword. If you started with shitty code, it will copy and paste that style. Therefore, it's worth making the first code you are writing as high quality as possible. Perhaps even iterating with <- -> ChatGPT or Copilot Chat to act as a code reviewer for asking for suggestions.
7. Using variable types. If you add types to your Python code or use TypeScript, rather than JavaScript, Copilot will be able to infer what you're trying to do, due to the types.
  - Copilot is really good at creating "converter" functions, which tend to be pretty tedious to write. Just by giving a function signature with typed inputs and outputs, Copilot will be able to figure out how to do the mapping.
8. Copilot tends to be really good at helping you figure out the next line. I find that the larger the block of code, the less you should trust it. If it's delivering an entire function to you that function rarely has a the correct implementation.
9. Iteration is key. Start with something small and keep adding to it.

# Challenges or Gotchas
1. Writing all of these specifc, inline comments is great. It feels like it adds readability to the code. However, if you ever change the implementation you now have two conflicting pieces of context. The comment and the actual code. So when the next developer comes along, they will have to figure out which one is correct. This is a problem with all comments that describe "what" the code is doing, but with copilot the tendency is to write more of these comments. So it's something to be aware of.
2. Copilot is great for code "in the small". It's not going to suggest how you should architect your code for the particular problem you're solving. For instance, it won't:
   - Identify when your class is getting too big and suggest you break it up.
   - Identify when you should be using a different design pattern.
   - Identify when you should be using a different data structure.
   - Tell you when you should be using a particular programming technqiue or pattern like dependency injection, or the factory pattern.
   - It won't help you manage your dependencies and watch to make sure you aren't creating a circular dependency.
3. I haven't figured out how to really use copilot when debugging. In Visual Studio, when you hit an exception, there's an "ask copilot" button but I haven't figured out how to use that well. [Here's a demo of that functionality](https://youtu.be/5pbPLHYB6-0?t=1513).
4. I still don't know how to use copilot to fix non-exception bugs. All of the code runs, but the logic of the various components fitting together generates the incorrect behaviour for the user. I haven't figured out how to use copilot to help me with that.

# Use Cases
1. Creating dictionaries with lookup data
2. Creating regular expressions based on comments
# References
[8 things you didn’t know you could do with GitHub Copilot](https://github.blog/2022-09-14-8-things-you-didnt-know-you-could-do-with-github-copilot/?utm_campaign=2024q1-em-MSFT-CopilotForIndividuals-VScom-LP-Body)
