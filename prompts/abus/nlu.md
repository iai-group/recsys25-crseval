| Intent (Code)                | Description                                                  | Example                                                      |
| ---------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Request Information (REQ)    | Recommender requests for the seeker's preference or feedback. | "What kind of movies do you like?"                         |
| Clarify Question (CLA)       | Recommender asks a clarifying question for more details.     | "What kind of animated movie are you thinking of?"         |
| Respond-Feedback (RES)       | Recommender responds to any other feedback from the seeker.  | "That's my favourite Christmas movie too! " (U: "My absolute favourite!!") |
| Answer (ANS)                 | Recommender answers the question asked by the seeker.        | "Steve Martin and John Candy." (Q: "Who is in that?")      |
| Recommend-Show (REC-S)       | Recommender provides recommendation by showing it directly.  | "The Invitation (2015) is a movie kids like."              |
| Recommend-Explore (REC-E)    | Recommender provides recommendation by inquiring about the seeker's preference. | "Have you seen Cult of Chucky (2017) that one as pretty scary." |
| Explain-Introduction (EXP-I) | Recommender explains recommendation with non-personalized introduction. | "What about Sleepless in Seattle (1993)? Hanks and Ryan?"  |
| Explain-Preference (EXP-P)   | Recommender explains recommendation based on the seeker's past preference. | "Will Ferrell is also very good in Elf (2003) if you're in need of another comedy" |
| Explain-Suggestion (EXP-S)   | Recommender explains recommendation in a suggestive way.     | "If you like gory then I would suggest The Last House on the Left (2009)." |
| Other (OTH)                  | Greetings, gratitude expression, or chit-chat utterances.    | "Have a good night."                                       |

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

Given the list of available intents and slots, extract a list of dialogue acts from a given utterance. A dialogue act is a pair of an intent and an optional list of slot-value pairs represented as intent_code(slot="value",slot,...) where the value of a slot is optional or taken from the utterance without any modifications. Multiple dialogue acts are separated by '|'. If no dialogue acts are found, say None. Strictly follow the specified format.

Example 1:
Input utterance: you're welcome.
Dialogue acts: OTH()

Example 2:
Input utterance: Hi, what kind of movies do you like?
Dialogue acts: OTH()|REQ(GENRE)

Example 3:
Input utterance: Okay! How about Horrible Bosses (2011) or Superbad (2007)?  
Dialogue acts: REC-S(TITLE='Horrible Bosses', TITLE='Superbad')

Example 4:
Input utterance: It came out in 2011...No problem! You're welcome!  
Dialogue acts: RES(YEAR="2011")|OTH()

Example 5:
Input utterance: how about Eddie Murphy Raw (1987) it is a stand up comedy  
Dialogue acts: REC-S(TITLE='Eddie Murphy Raw')|EXP-I(GENRE='stand up comedy')

Input utterance: {utterance}  
Dialogue acts:
