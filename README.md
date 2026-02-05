# Limitations of Current Evaluation Practices for Conversational Recommender Systems and the Potential of User Simulation

This repository provides resources developed within the following article [[PDF](https://dl.acm.org/doi/pdf/10.1145/3767695.3769478)]:

> Nolwenn Bernard and Krisztian Balog. 2025. Limitations of Current Evaluation Practices for Conversational Recommender Systems and the Potential of User Simulation. In Proceedings of the 2025 Annual International ACM SIGIR Conference on Research and Development in Information Retrieval in the Asia Pacific Region (SIGIR-AP 2025). Association for Computing Machinery, New York, NY, USA, 261–271. [DOI: 10.1145/3767695.3769478](https://doi.org/10.1145/3767695.3769478)

## Summary

Research and development on conversational recommender systems (CRSs) critically depends on sound and reliable evaluation methodologies. However, the interactive nature of these systems poses significant challenges for automatic evaluation. This paper critically examines current evaluation practices for CRSs and identifies two key limitations: the over-reliance on static test collections and the inadequacy of existing evaluation metrics. To substantiate this critique, we analyze real user interactions with nine existing CRSs and demonstrate a striking disconnect between self-reported user satisfaction and the performance scores reported in prior literature.
To address these limitations, this work explores the potential of user simulation to generate dynamic interaction data, offering a departure from static datasets. Furthermore, we propose novel evaluation metrics designed to better align with real user satisfaction. Our analysis of different simulation approaches provides valuable insights into their effectiveness and reveals promising initial results, showing improved correlation with system rankings compared to traditional evaluation methods. While these findings indicate a significant step forward in CRS evaluation, we also identify areas for future research and refinement in both simulation techniques and evaluation metrics.

## Repository Structure

This repository is structured as follows:

  - `prompts/abus`: folder with prompts used for the agenda-based user simulator, ABUS.
  - `prompts/llm-us`: folder with prompts used for the LLM-based user simulator, LLM-US.

## Citation

If you use the resources presented in this repository, please cite:

```bibtex
@inproceedings{Bernard:2025:SIGIRAP,
  author = {Bernard, Nolwenn and Balog, Krisztian},
  title = {Limitations of Current Evaluation Practices for Conversational Recommender Systems and the Potential of User Simulation},
  year = {2025},
  doi = {10.1145/3767695.3769478},
  booktitle = {Proceedings of the 2025 Annual International ACM SIGIR Conference on Research and Development in Information Retrieval in the Asia Pacific Region},
  pages = {261--271},
  series = {SIGIR-AP '25},
  publisher = {Association for Computing Machinery},
}
```

## Contact

Should you have any questions, please contact Nolwenn Bernard at [nolwenn-bernard@th-koeln.de](mailto:nolwenn-bernard@th-koeln.de).
