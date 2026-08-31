<p align="center">
<h1 align="center">Near-Miss Context Contamination and Language-Asymmetric Evidence Arbitration in LLMs</h1>

<p align="center">
<strong>Jebish Purbey</strong><sup>1, 2</sup>,
<strong>Sanjeeb Prasad Panday</strong><sup>2</sup>,
<strong>Barnnita Shrestha</strong><sup>3</sup>,
<strong>Bikash Balami</strong><sup>4</sup>,
<strong>Aakash Pandey</strong><sup>1</sup>,
<strong>Bibek Khanal</strong><sup>5</sup>
</p>

<p align="center">
<sup>1</sup>Dogma Group &nbsp;&nbsp;
<sup>2</sup>Pulchowk Campus, Tribhuvan University &nbsp;&nbsp;
<sup>3</sup>Asian Institute of Technology &nbsp;&nbsp;
<sup>4</sup>CDCSIT, Tribhuvan University &nbsp;&nbsp;
<sup>5</sup>IoE, Tribhuvan University
</p>

This repository accompanies our paper studying two generator-side failure modes in retrieval-augmented factual question answering:

- **Near-miss context contamination**: true, relation-matched context about the *wrong* entity (e.g. a sentence about Bhutan for a question about Nepal) can still shift a model's answer, even with no explicit contradiction present.
- **Language-asymmetric evidence arbitration**: when English and local-language evidence disagree, models show a content-independent preference for one language's evidence over the other that reverses by model family, and a label-only control shows models over-trust evidence tagged as English even when both snippets are written in English.

Both probes are built on controlled, constructed evidence rather than live retrieval, evaluated across four models (GPT-5.4, GPT-5.4-mini, DeepSeek-V4-Pro, DeepSeek-V4-Flash) on [Mintaka](https://github.com/amazon-science/mintaka) and [PopQA](https://github.com/AlexTMallen/adaptive-retrieval), including Nepali and Hindi translations produced and verified for this work.

## License

The Mintaka-derived translations are released under Mintaka's own Creative Commons Attribution 4.0 license, and the PopQA-derived translations are released under PopQA's MIT license. The sentence-embedding model used for near-neighbor selection (`all-MiniLM-L6-v2`) is released under the Apache 2.0 license.

## Contact

- Jebish Purbey: jebishpurbey@gmail.com
- Sanjeeb Prasad Panday: sanjeeb@ioe.edu.np
