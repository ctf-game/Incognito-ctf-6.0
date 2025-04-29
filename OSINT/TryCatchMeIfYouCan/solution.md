# CTF Writeup: TraceMeIfYouCan

## Challenge Overview
In this challenge, we are tasked with investigating a series of user identities across different platforms. The goal is to identify key clues that will eventually lead us to the flag hidden in the user bio.

## Challenge Description
```
I always forget my usernames, so I’m writing one here to remember... Sha4owM1rker
``` 

### Key Information:
1. **Reddit User: Sha4owM1rker**
   - Reddit Bio: "We don't have the whole month for this; we need to achieve it today! You are very close."
   - **Notice the Typo**: There's a subtle typo in the word "achieve" – a potential clue.
   - **Clue**: Archive-related, as indicated by the typo.

2. **archive.today**
   - User Comment: "I am also known as M1rk5rSh14ow in past."
   - This suggests the user has gone by the name "M1rk5rSh14ow" in previous contexts. 

3. **Telegram Username**: M1rk5rSh14ow
   - The same username appears on Telegram, providing continuity between the platforms.

4. **User Bio on Telegram**: The bio contains the **flag**. 

---

## Strategy and Analysis

### Step 1: Identify the Key Platforms
The key platforms involved are:
- **Reddit**
- **archive.today**
- **Telegram**

### Step 2: Understanding the Clue from Reddit
- The Reddit user's bio contains a typo: "achieve" is spelled "achive". This could indicate that something was missed or left out intentionally—perhaps an archive-related clue.
- The mention of "archive" might hint towards using archive services like archive.today to trace past activity or find hidden information.

### Step 3: Investigating archive.today
- The comment on archive.today indicates that the user was previously known as **M1rk5rSh14ow**. This historical name change could be key to uncovering past activity, as it suggests they might have left behind useful traces.
- The connection between **Sha4owM1rker** and **M1rk5rSh14ow** is essential, as the latter is the username on Telegram, and could have more relevant information hidden in the user’s bio.

### Step 4: Telegram Bio Analysis
- Upon visiting the Telegram profile, we discover the flag hidden in the user's bio. This is the final step in solving the challenge. The flag is typically a string in the format `CTF{...}`.

---

## Flag

After piecing together the clues from Reddit, archive.today, and Telegram, the final solution reveals the **flag**. We won’t reveal the exact flag here, but it’s directly available in the Telegram user's bio once the user is identified correctly.

---

## Conclusion
The challenge required identifying a typo in the Reddit bio as a hint for using archive services, tracking a historical username across platforms, and ultimately discovering the flag hidden in the Telegram bio. By following the trail from one platform to another, we were able to unlock the flag.

**Pro Tip**: Always pay attention to typos, they can sometimes be the most significant clue in a CTF challenge!
