# 💭 Reflection: Game Glitch Investigator

## 1. What was broken when you started?

The game looked good when I first ran it, but after I started playing, I noticed several problems. The hint system kept telling me to guess a lower number every time I entered a guess. Eventually, I reached 0, but the game still said "lower," even though the instructions said the secret number should be between 0 and 100. This made it impossible to find the correct answer.

Two other bugs I noticed were related to restarting the game and the attempts counter. The **New Game** button did not work properly because the game would not fully reset after the first round. The secret number seemed to stay the same until I refreshed the page. I also noticed that the attempts counter went into negative numbers, such as **-3**, on both Easy and Hard difficulty levels. In addition, the **Show Hint** checkbox did not appear to do anything because hints were shown whether the option was checked or not.

## Bug Reproduction Log

| Input / Action                                 | Expected Behavior                                                           | Actual Behavior                                             | Console Output / Error |
| ---------------------------------------------- | --------------------------------------------------------------------------- | ----------------------------------------------------------- | ---------------------- |
| Keep guessing numbers until reaching 0         | The game should provide correct hints and stop when no valid guesses remain | The hint continued saying "Lower" even when the guess was 0 | No error shown         |
| Click **New Game** after finishing a round     | The game should reset with a new secret number                              | The game did not fully reset until the page was refreshed   | No error shown         |
| Select Easy or Hard mode and continue guessing | Attempts should decrease to 0 and stop                                      | Attempts continued into negative values (for example, -3)   | No error shown         |
| Check and uncheck the **Show Hint** option     | Hints should only appear when enabled                                       | Hints appeared regardless of the checkbox state             | No error shown         |


## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
