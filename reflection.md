# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
When I first ran the game, it appeared functional on the surface, but the  gameplay loop was broken. Clicking the new game button didn't clear out old scores which locked the game if you had previously won or lost. I also noticed two  bugs immediately. The hints were giving me the exact opposite advice and my attempt counter was starting at 7 instead of 8 on normal difficulty.

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|guess = 50 |guess lower |guess lower |none |
|guess = 50 |returns guess higher, displays guess lower   |return and display the same thing |none |
|guess = 50 |returns guess higher | displays guess higher|  |

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)? I used gemini
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
One example of where the AI was correct was the how the number of tries shown in the front end was consistently off by one, but in the backened the user had 7 tries, and I verified it by running the code and counting. 
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
The AI suggestions that were misleading were the vscode's suggestions that had nothing to do with the actual assignment itself, rather it was predicting what I could be typing. I simply turned it off. 

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
In order to decide if a bug was fixed, I first identified what the bug was and then viewing the code, after fixing the code I had checked if the backend aligned with the front end, and if everything was in order then it was fine.
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  One test that I ran was check_guess(50,20), and making sure that it displayed too high.
- Did AI help you design or understand any tests? How?
AI didn't help me understand the tests but rather it helped me open my eyes to more aspects of projects to pay more attention to.

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
Streamlit doesn't just update a single button when you click it; it reruns the  Python script. Because of this, variables will reset to their default values on every click unless you explicitly hide them in the st.session_state dictionary.
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
One habit that I would reuse is consistently cross checking what I told the AI to do vs what it actually did and actually looking at tthe source code.
- This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
I would try and take more intiative and try and figure out the logic of everything first and make a tracklist of things to add/change before I begin to use AI.
- In one or two sentences, describe how this project changed the way you think about AI generated code.
This project changed the way I thought about AI generated code because it made me realize that AI can make plenty of mistakes and not to overrely on it.
