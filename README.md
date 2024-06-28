# RAG-Limitations-LLM
#### Spring 2024, CSE 256: Statistical Natural Language Processing, UC San Diego

Working with Large Language Models (LLMs) presents several challenges, including gaps in domain knowledge, issues with factual accuracy, and the problem of hallucination. Retrieval Augmented Generation (RAG) offers a solution to alleviate some of these challenges by enhancing LLMs with external knowledge sources such as databases. When the user asks the LLM-based chatbot a question, documents related to that user’s question are retrieved from a database and prepended to the user’s query as additional context, allowing the LLM to consider that context in generating its response. Clearly, this approach has several advantages over the standard (without RAG) approach:
1. Additional context ‘guardrails’ the LLM and reduces the chances of hallucinations.
2. The retrieved information is especially beneficial in domain-specific applications where it allows the
LLM to generate more refined, accurate, and upto-date results.
3. The database can be modified and updated without the need to retrain the LLM.

In this project, perform a detailed analysis to understand the limitations of the existing RAG systems, and identify and provide concrete examples of failure cases. These include managing unrelated noise from external sources, handling mathematical reasoning, effectively integrating information, interpreting negative or missing statements, dealing with conflicting knowledge, and the difficulty of evaluating these systems. These challenges often result in irrelevant, inaccurate, or incoherent responses.

To address these limitations, researchers are exploring several avenues. Enhanced context management techniques and architectures, such as Mamba SSM, aim to help models better understand full conversation histories. Noise reduction methods, like Graph RAG, seek to filter out irrelevant details by leveraging structured entity information. New evaluation metrics are being developed to more accurately assess the relevance, diversity, and factual accuracy of responses. Additionally, incorporating symbolic reasoning capabilities could enable RAG models to handle mathematical problems more effectively.

## Links
[Report](Project_Report.pdf)

## References
1. Ahn, J., Verma, R., Lou, R., Liu, D., Zhang, R., and Yin, W. (2024). Large language models for mathematical reasoning: Progresses and challenges.
2. Bird, S. and Loper, E. (2004). NLTK: The natural language toolkit. In Proceedings of the ACL Interactive Poster and Demonstration Sessions, pages 214–217, Barcelona, Spain. Association for Computational Linguistics.
3. Borgeaud, S., Mensch, A., Hoffmann, J., Cai, T., Rutherford, E., Millican, K., van den Driessche, G., Lespiau, J.-B., Damoc, B., Clark, A., de Las Casas, D., Guy, A., Menick, J., Ring, R., Hennigan, T., Huang, S., Maggiore, L., Jones, C., Cassirer, A., Brock, A., Paganini, M., Irving, G., Vinyals, O., Osindero, S., Simonyan, K., Rae, J.W., Elsen, E., and Sifre, L. (2022). Improving language models by retrieving from trillions of tokens.
4. Boteva, V., Gholipour, D., Sokolov, A., and Riezler, S. (2016). A full-text learning to rank dataset for medical information retrieval. In Ferro, N., Crestani, F., Moens, M.-F., Mothe, J., Silvestri, F., Di Nunzio, G. M., Hauff, C., and Silvello, G., editors, Advances in Information Retrieval, pages 716–722, Cham. Springer International Publishing.
5. Chen, J., Lin, H., Han, X., and Sun, L. (2023). Benchmarking large language models in retrieval-augmented generation.
6. Douze, M., Guzhva, A., Deng, C., Johnson, J., Szilvasy, G., Mazar´e, P.-E., Lomeli, M., Hosseini, L., and J´egou, H. (2024). The faiss library.
7. Edge, D., Trinh, H., Cheng, N., Bradley, J., Chao, A., Mody, A., Truitt, S., and Larson, J. (2024). From local to global: A graph rag approach to query-focused summarization.
8. Es, S., James, J., Espinosa-Anke, L., and Schockaert, S. (2023). Ragas: Automated evaluation of retrieval augmented generation.
9. Gao, Y., Xiong, Y., Gao, X., Jia, K., Pan, J., Bi, Y., Dai, Y., Sun, J., Wang, M., and Wang, H. (2024). Retrieval-augmented generation for large language models: A survey.
10. Gu, A. and Dao, T. (2024). Mamba: Linear-time sequence modeling with selective state spaces.
11. Hoshi, Y., Miyashita, D., Ng, Y., Tatsuno, K., Morioka, Y., Torii, O., and Deguchi, J. (2023). Ralle: A framework for developing and evaluating retrieval-augmented large language models.
12. Hu, Y., Lei, Z., Zhang, Z., Pan, B., Ling, C., and Zhao, L. (2024). Grag: Graph retrieval-augmented generation.
13. Izacard, G. and Grave, E. (2021). Leveraging passage retrieval with generative models for open domain question answering.
14. Kalai, A. T. and Vempala, S. S. (2024). Calibrated language models must hallucinate.
15. Karpukhin, V., Oguz, B., Min, S., Lewis, P., Wu, L., Edunov, S., Chen, D., and Yih, W.-t. (2020). Dense passage retrieval for open-domain question answering. In Proceedings of the 2020 Conference on Empirical Methods in Natural Language Processing (EMNLP), pages 6769–6781, Online. Association for Computational Linguistics.
16. Lewis, P., Perez, E., Piktus, A., Petroni, F., Karpukhin, V., Goyal, N., K¨uttler, H., Lewis, M., tau Yih, W., Rockt¨aschel, T., Riedel, S., and Kiela, D. (2021). Retrieval-augmented generation for knowledge-intensive nlp tasks.
17. Liu, N. F., Lin, K., Hewitt, J., Paranjape, A., Bevilacqua, M., Petroni, F., and Liang, P. (2023a). Lost in the middle: How language models use long contexts.
18. Liu, Y., Huang, L., Li, S., Chen, S., Zhou, H., Meng, F., Zhou, J., and Sun, X. (2023b). Recall: A benchmark for llms robustness against external counterfactual knowledge.
19. Saad-Falcon, J., Khattab, O., Potts, C., and Zaharia, M. (2024). Ares: An automated evaluation framework for retrieval-augmented generation systems.
20. Tay, Y., Dehghani, M., Bahri, D., and Metzler, D. (2022). Efficient transformers: A survey.
21. Wachsmuth, H., Syed, S., and Stein, B. (2018). Retrieval of the best counterargument without prior topic knowledge. In Gurevych, I. and Miyao, Y., editors, Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers), pages 241–251, Melbourne, Australia. Association for Computational Linguistics.
22. Wang, B., Ping,W., Xu, P., McAfee, L., Liu, Z., Shoeybi, M., Dong, Y., Kuchaiev, O., Li, B., Xiao, C., Anandkumar, A., and Catanzaro, B. (2023). Shall we pretrain autoregressive language models with retrieval? a comprehensive study.
23. Wang, X., Wang, J., Cao, W., Wang, K., Paturi, R., and Bergen, L. (2024). Birco: A benchmark of information
retrieval tasks with complex objectives.
24. Yu, F. (2024). Why vector search didn’t work for your rag solution?
25. Zhao, P., Zhang, H., Yu, Q.,Wang, Z., Geng, Y., Fu, F., Yang, L., Zhang, W., Jiang, J., and Cui, B. (2024). Retrieval-augmented generation for ai-generated content: A survey.
