# Prompts for ABUS

This folder contains the different prompts used for natural language understanding (NLU) and generation (NLG) components of ABUS. These prompts aim to leverage in-context learning abilities of large language models (LLM). That is, they are structured similarly to include a description of the intents and slots used in the dialogue acts, a description of the task to execute, and examples of the expected input and output.

The taxonomy of intents and the examples used in the prompts are taken from the [IARD dataset](https://github.com/wanlingcai1997/umap_2020_IARD).

  * [NLU prompt](nlu.md): This prompt is used to extract dialogue acts from the utterances issued by the CRS agent.
  * [NLG prompt](nlg.md): This prompt is used to translate a list of dialogue acts into a coherent and natural language utterance.
