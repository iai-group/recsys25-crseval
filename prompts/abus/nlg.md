| Intent (Code)              | Description                                                  | Example                                                      |
| -------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Initial Query (IQU)        | Seeker asks for a recommendation in the first query.         | "I like comedy do you know of any good ones?"              |
| Continue (CON)             | Seeker asks for more recommendations in the subsequent query. | "Do you have any other suggestions?"                       |
| Reformulate (REF)          | Seeker restates her/his query with or without clarification/further constraints. | "Maybe I am not being clear. I want something that is in the theater now." |
| Start Over (STO)           | Seeker starts a new query to ask for recommendations.        | "Anything that I can watch with my kids under 10."         |
| Provide Preference (PRO)   | Seeker provides specific preference for the item s/he is looking for. | "I usually enjoy movies with Seth Rogen and Jonah Hill."   |
| Answer (ANS)               | Seeker answers the question issued by the recommender.       | "Maybe something with more action." (Q: "What kind of fun movie you look for?") |
| Ask Opinion (ASK)          | Seeker asks the recommender's personal opinions.             | "I really like Reese Witherspoon. How about you?"          |
| Seen (SEE)                 | Seeker has seen the recommended item before.                 | "I have seen that one and enjoyed it."                     |
| Accept (ACC)               | Seeker likes the recommended item.                           | "Awesome, I will check it out."                            |
| Reject (REJ)               | Seeker dislikes the recommended item.                        | "I hated that movie. I did not even crack a smile once."   |
| Inquire (INQ)              | Seeker wants to know more about the recommended item.        | "I haven't seen that one yet. What's it about?"            |
| Critique-Feature (CRI-F)   | Seeker makes critiques on specific features of the current recommendation. | "That's a bit too scary for me."                           |
| Critique-Add (CRI-A)       | Seeker adds further constraints on top of the current recommendation. | "I would like something more recent."                      |
| Neutral Response (NRE)     | Seeker does not indicate her/his preference for the current recommendation. | "I have actually never seen that one."                     |
| Critique-Compare (CRI-C)   | Seeker requests sth similar to the current recommendation in order to compare. | "Den of Thieves (2018) sounds amazing. Any others like that?" |
| Other (OTH)                | Greetings, gratitude expression, or chit-chat utterances.    | "Sorry about the weird typing."                            |

| Slot |
| ---- |
| GENRE |
| TITLE |
| PLOT |
| ACTOR |
| DIRECTOR |
| RATING |
| KEYWORDS |
| YEAR |
| OTHER |

Generate a user utterance that corresponds to the given dialogue acts. The generated utterance should be straight to the point and include all the information provided in the dialogue acts. A dialogue act is a pair with an intent and an optional list of slot-value pairs. A description of the intents and slots is provided in the tables above.

Example 1:
Dialogue acts: REJ(GENRE='horror')|CRI-A(GENRE='thrillers')
Generated utterance: I don't really like horror movies what about thrillers

Example 2:
Dialogue acts: OTH()
Generated utterance: Thank you bye.

Example 3:
Dialogue acts: PRO(TITLE="The Parent Trap")|SEE()|CRI-A(GENRE="animated")  
Generated utterance: I like things like The Parent Trap...Oh yeah that was a good one. the kids enjoyed it too....maybe something not animated

Example 4:
Dialogue acts: INQ(TITLE="The River Wild", PLOT)
Generated utterance: I haven't seen The River Wild. What's that about?

Example 5:
Dialogue acts: ACC()  
Generated utterance: Yes. oh okay. I'll check it out. Thanks!

Dialogue acts: {dialogue_acts}  
Generated utterance:
