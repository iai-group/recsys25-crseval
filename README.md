# Limitations of Current Evaluation Practices for Conversational Recommender Systems and the Potential of User Simulation

This repository provides the prompts used in the paper **Limitations of Current Evaluation Practices for Conversational Recommender Systems and the Potential of User Simulation**.

## Summary

Research and development on conversational recommender systems (CRSs) critically depends on sound and reliable evaluation methodologies. However, the interactive nature of these systems poses significant challenges for automatic evaluation. This paper critically examines current evaluation practices for CRSs and identifies two key limitations: the over-reliance on static test collections and the inadequacy of existing evaluation metrics. To substantiate this critique, we analyze real user interactions with nine existing CRSs and demonstrate a striking disconnect between self-reported user satisfaction and the performance scores reported in prior literature.
To address these limitations, this work explores the potential of user simulation to generate dynamic interaction data, offering a departure from static datasets. Furthermore, we propose novel evaluation metrics designed to better align with real user satisfaction. Our analysis of different simulation approaches provides valuable insights into their effectiveness and reveals promising initial results, showing improved correlation with system rankings compared to traditional evaluation methods. While these findings indicate a significant step forward in CRS evaluation, we also identify areas for future research and refinement in both simulation techniques and evaluation metrics.

## Repository Structure

This repository is structured as follows:

  - `prompts/abus`: folder with prompts used for the agenda-based user simulator, ABUS.
  - `prompts/llm-us`: folder with prompts used for the LLM-based user simulator, LLM-US.
