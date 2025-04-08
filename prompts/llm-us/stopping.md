As a USER interacting with an ASSISTANT to receive a recommendation, analyze the conversation history to determine if it is progressing productively. If the conversation has been stuck in a loop with repeated misunderstandings across multiple turns, return 'FALSE' to indicate the conversation should be terminated. Otherwise, return'TRUE' to indicate that the conversation should continue. Only return 'TRUE' or'FALSE' without any additional information.

HISTORY:  
{conversation_history}

Continue?
