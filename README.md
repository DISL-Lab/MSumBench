<h1 align="center">
MSumBench
</h1>

<h3 align="center">
Towards Multi-dimensional Evaluation of LLM Summarization across Domains and Languages
</h3>

<div align="center">
  <p>Authors: Hyangsuk Min, Yuho Lee, Minjeong Ban, Jiaqi Deng, Nicole Hee-Yeon Kim, Taewon Yun, Hang Su, Jason Cai, Hwanjun Song</p>
  <a href="https://arxiv.org/abs/2506.00549">
  <img src="https://img.shields.io/badge/arXiv-b31b1b?style=flat-square" alt="arXiv">
  </a>
  <a href="https://disl-lab.github.io/">
  <img src = "https://img.shields.io/badge/Data%20Intelligence%20System%20Lab-B552CB.svg?logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBzdGFuZGFsb25lPSJubyI/Pgo8IURPQ1RZUEUgc3ZnIFBVQkxJQyAiLS8vVzNDLy9EVEQgU1ZHIDIwMDEwOTA0Ly9FTiIKICJodHRwOi8vd3d3LnczLm9yZy9UUi8yMDAxL1JFQy1TVkctMjAwMTA5MDQvRFREL3N2ZzEwLmR0ZCI+CjxzdmcgdmVyc2lvbj0iMS4wIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiB3aWR0aD0iNTQ0LjAwMDAwMHB0IiBoZWlnaHQ9IjU0MS4wMDAwMDBwdCIgdmlld0JveD0iMCAwIDU0NC4wMDAwMDAgNTQxLjAwMDAwMCIKIHByZXNlcnZlQXNwZWN0UmF0aW89InhNaWRZTWlkIG1lZXQiPgoKPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsNTQxLjAwMDAwMCkgc2NhbGUoMC4xMDAwMDAsLTAuMTAwMDAwKSIKZmlsbD0iIzAwMDAwMCIgc3Ryb2tlPSJub25lIj4KPHBhdGggZD0iTTExNDggNDQzOSBsLTMgLTk1MSAtNzMgLTE5IGMtNTQwIC0xMzcgLTk1NSAtNTk0IC0xMDM2IC0xMTQxIC0xMTEKLTc0NyAzODUgLTE0NDQgMTEyOSAtMTU4NCA2NyAtMTIgMTY4IC0xOCAzOTMgLTIxIGwzMDIgLTUgMCAtMzU1IDAgLTM1NSA1NjgKNSBjNDQ1IDMgNTkwIDggNjcyIDIwIDQ4NyA3MiA5MjYgMjYxIDEzMDAgNTU3IDEyNCA5OCAzMzggMzEwIDQzNCA0MzAgMjc3CjM0NyA0NzggNzk2IDU1MCAxMjMwIDQxIDI0NSA0NiA1OTUgMTEgODI4IC02OSA0NzQgLTI2OCA5MzUgLTU2MSAxMzAyIC04NwoxMDkgLTMxNSAzMzcgLTQyNCA0MjQgLTMxNSAyNTEgLTY5MSA0MzEgLTEwOTEgNTIyIC0yNTUgNTcgLTI0OSA1NyAtMTI0NiA2MQpsLTkyMyA0IC0yIC05NTJ6IG0xOTQyIDU5NyBjNDEzIC02OSA3OTYgLTIzNyAxMTA1IC00ODQgODIzIC02NjAgMTExNCAtMTc1Nwo3MjYgLTI3MzUgLTE3MCAtNDI3IC00OTcgLTgyNSAtODk2IC0xMDkxIC0zMDUgLTIwNCAtNjg4IC0zMzkgLTEwNTkgLTM3NSAtNjAKLTYgLTI1OSAtMTEgLTQ0MyAtMTEgbC0zMzMgMCAwIDE5MCAwIDE5MCAyOTggMCBjNDQwIDAgNjE4IDIyIDg3MCAxMDYgMjg0IDk1CjUyMyAyNDAgNzQ1IDQ1MyAyNjAgMjUwIDQzNSA1NDYgNTM3IDkwOSA4NiAzMDQgODcgNjg4IDQgMTAwOCAtMjIzIDg1OSAtMTAwMgoxNDcxIC0xODc5IDE0NzcgLTk4IDAgLTE2MiAtNSAtMjE0IC0xNiAtMzE5IC03MyAtNTYzIC0zMDAgLTY1NyAtNjE0IC0yNSAtODEKLTI3IC0xMDYgLTMyIC0zMDUgbC00IC0yMTggLTEzNyAwIGMtNzUgMCAtMTYwIC0zIC0xODggLTYgbC01MyAtNyAwIDc3NyAwCjc3NyA3NTMgLTQgYzY2MCAtMyA3NjUgLTUgODU3IC0yMXogbS0xNzAgLTcwMSBjOTQ1IC0xMTAgMTU5NiAtOTg0IDE0MzQKLTE5MjUgLTE5IC0xMTQgLTc5IC0yOTkgLTEzMiAtNDEyIC0yMTAgLTQ0OCAtNjE2IC03NzkgLTExMDcgLTkwMiAtMTM3IC0zNQotMjkwIC00NiAtNjExIC00NiBsLTMxNCAwIDAgMTk1IDAgMTk1IDMyOSAwIGMzOTkgLTEgNDc2IDkgNjc4IDg2IDIyNSA4NiA0NDcKMjY2IDU4OCA0NzggMjE1IDMyNCAyNjcgNzQwIDEzOCAxMTEwIC00MiAxMjEgLTY5IDE3NSAtMTQxIDI4NiAtNjggMTA0IC0yNDAKMjc4IC0zMzcgMzQyIC0yMTIgMTM5IC00NTkgMjE4IC02ODAgMjE4IC02OSAwIC04NyAtNCAtMTE1IC0yMiAtNzggLTUzIC0xMDAKLTEzOCAtNTggLTIxNyAzNCAtNjMgNzUgLTgxIDIwMyAtOTEgMzY0IC0zMCA2NTYgLTI0MCA4MDAgLTU3NyA0NyAtMTEwIDY4Ci0yMTcgNjkgLTM1MyAxIC0zNjIgLTIwMCAtNjgyIC01MjggLTg0MCAtMTc2IC04NCAtMjY4IC05OCAtNjczIC05OSBsLTI3MyAtMgowIDEwNTkgYzAgOTA1IDIgMTA2NiAxNSAxMTE1IDUxIDE5OCAyMTggMzU5IDQxNSA0MDEgODYgMTkgMTQ5IDE5IDMwMCAxegptLTEwNjIgLTE4NTcgbC0zIC03MTMgLTU3IDMgYy0xMzMgNiAtMjUzIDg5IC0yOTYgMjA1IC0yMiA1NyAtMjIgNjggLTIyIDYzNwpsMCA1ODAgMTkwIDAgMTkwIDAgLTIgLTcxMnogbS03MDggMTA1IGMwIC02MzggMCAtNjM2IDcyIC03ODMgMzMgLTY3IDYwIC0xMDIKMTIzIC0xNjUgMTIzIC0xMjQgMjQ5IC0xODEgNDIwIC0xOTQgbDkwIC02IDMgLTE5MyAyIC0xOTQgLTMwMiA1IGMtMjI0IDQKLTMyMCA5IC0zNjggMjAgLTQyOSAxMDIgLTc1MiA0MzYgLTgyNSA4NTQgLTE5IDEwOCAtMTkgMjc0IC0xIDM3OCA2NyAzNzggMzQzCjY5OCA3MTEgODI0IDMzIDExIDYzIDIwIDY4IDIxIDQgMCA3IC0yNTUgNyAtNTY3eiIvPgo8L2c+Cjwvc3ZnPgo=&style=flat-square">
  </a>
  
<p align="center">
  <img src="https://github.com/user-attachments/assets/4dfaef99-3703-43ea-b0a2-b0def5920d71" alt="" width="1000">
</p>

</div>

---

This is the official github repository for "Towards Multi-dimensional Evaluation of LLM Summarization across Domains and Languages"

---

# 📖 Data Description

We provide samples in MSumBench, which is available in `data`.

## Metadata
The metadata provides basic information about UniSumEval. All attributes are included in every file. Below is a description of each attribute. 

| Field       | Description                                |
|-------------|--------------------------------------------|
| uid         | Dataset unique ID                |
| doc_id      | ID in source dataset                       |
| dataset     | Source dataset name                        |
| domain      | Domain                                     |
| summary_model       | Summarizer name                            |
| summary     | Model summary        |
| fv_faithfulness     | faithfulness score from fact verification         |
| ka_completeness     | completeness score from key-fact alignment         |
| ka_conciseness     | conciseness score from key-fact alginment         |

# 🖇️ Citation

Please consider citation if our paper is useful in your research.
```BibTeX
@article{min2025towards,
  title={Towards Multi-dimensional Evaluation of LLM Summarization across Domains and Languages},
  author={Min, Hyangsuk and Lee, Yuho and Ban, Minjeong and Deng, Jiaqi and Kim, Nicole Hee-Yeon and Yun, Taewon and Su, Hang and Cai, Jason and Song, Hwanjun},
  journal={arXiv preprint arXiv:2506.00549},
  year={2025}
}
```

# 🤗 Acknowledgement
This work was supported by Institute of Information & communications Technology Planning & Evaluation (IITP), and partly supported by the National Research Foundation of Korea (NRF).

###### *This work was done @ KAIST Data Intelligence System Lab*
