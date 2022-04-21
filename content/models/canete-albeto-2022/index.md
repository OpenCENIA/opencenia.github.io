---
title: "ALBETO and DistilBETO: Lightweight Spanish Language Models"
date: 2022-01-01
publishDate: 2022-04-18T22:08:23.748893Z
authors:
- José Cañete
- Sebastián Donoso
- Felipe Bravo-Marquez
- Andrés Carvallo
- Vladimir Araujo
publication_types: ["1"]
abstract: "In recent years there have been considerable advances in pre-trained language models, where non-English language versions have also been made available. Due to their increasing use, many lightweight versions of these models (with reduced parameters) have also been released to speed up training and inference times. However, versions of these lighter models (e.g., ALBERT, DistilBERT) for languages other than English are still scarce. In this paper we present ALBETO and DistilBETO, which are versions of ALBERT and DistilBERT pre-trained exclusively on Spanish corpora. We train several versions of ALBETO ranging from 5M to 223M parameters and one of DistilBETO with 67M parameters. We evaluate our models in the GLUES benchmark that includes various natural language understanding tasks in Spanish. The results show that our lightweight models achieve competitive results to those of BETO (Spanish-BERT) despite having fewer parameters. More specifically, our larger ALBETO model outperforms all other models on the MLDoc, PAWS-X, XNLI, MLQA, SQAC and XQuAD datasets. However, BETO remains unbeaten for POS and NER. As a further contribution, all models are publicly available to the community for future research."
featured: true
publication: "*Proceedings of the 13th Edition of The Language Resources and Evaluation Conference (LREC), Marseille, France.* (to appear)"
url_pdf: https://arxiv.org/abs/2204.09145
url_code: https://github.com/OpenCENIA/lightweight-spanish-language-models
# url_slides: https://docs.google.com/presentation/d/17XHKoOTh_GwY4ZziEBH4qWJl8BkJ4P98HXxZAmUwR6g/edit#slide=id.g7fa90aae96_0_23
# url_video: https://pml4dc.github.io/iclr2020/program/pml4dc_10.html
links:
- name: Models
  url: https://huggingface.co/CenIA
- name: arXiv
  url: https://arxiv.org/abs/2204.09145
---

In recent years there have been considerable advances in pre-trained language models, where non-English language versions have also been made available. Due to their increasing use, many lightweight versions of these models (with reduced parameters) have also been released to speed up training and inference times. However, versions of these lighter models (e.g., ALBERT, DistilBERT) for languages other than English are still scarce. In this paper we present ALBETO and DistilBETO, which are versions of ALBERT and DistilBERT pre-trained exclusively on Spanish corpora. We train several versions of ALBETO ranging from 5M to 223M parameters and one of DistilBETO with 67M parameters. We evaluate our models in the GLUES benchmark that includes various natural language understanding tasks in Spanish. The results show that our lightweight models achieve competitive results to those of BETO (Spanish-BERT) despite having fewer parameters. More specifically, our larger ALBETO model outperforms all other models on the MLDoc, PAWS-X, XNLI, MLQA, SQAC and XQuAD datasets. However, BETO remains unbeaten for POS and NER. As a further contribution, all models are publicly available to the community for future research.