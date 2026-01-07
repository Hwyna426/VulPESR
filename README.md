# VulPESR
VulPESR is a vulnerability detection method that integrates semantic topology enhancement with chain-of-thought reasoning to achieve transparent and traceable vulnerability identification in C/C++ source code.

# Approach
![image-20241125191551680](Figs/Fig_1.png)

## Access to datasets

BigVul [1]: https://drive.google.com/drive/folders/1lUVArHAuXybDOCt-UdsMqguhN-DE6eEM?usp=drive_link

Devign [2]: https://drive.google.com/drive/folders/1xohZNUlfmUc-I248c4q2IM2fcpL635mW?usp=drive_link

## Figure

We put the images involved in the paper in the folder `Figs\` 

## Install dependencies

Please install them first.

```
unzip VulPESR.zip
cd VulPESR_main
conda create -n vulpesr python=3.9 
conda activate vulpesr
pip install -r requirements.txt
```
## About the Models

In the replication, we provide:

* `analyze_cpg.scala` : Used to extract code analysis graphs
* `convert_data.py` : Used to format data
* `agument_data.py` : Used to augment training data
* `finetuning.py` : Used to fine-tune LLMs
* `inference.py` : Used for chain-of-thought reasoning
* `./to_graph` : Used to process data

## References

[1] Yaqin Zhou, Shangqing Liu, Jingkai Siow, Xiaoning Du, and Yang Liu. Devign: Effective vulnerability identification by learning comprehensive program semantics via graph neural networks. *Advances* *in neural information processing systems*, 32, 2019. https://doi.org/10.48550/arXiv.1909.03496.

[2]J. Zhang, S. Liu, X. Wang, T. Li, and Y. Liu, “Learning to locate and describe vulnerabilities,” in 2023 38th IEEE/ACM International Conference on Automated Software Engineering (ASE). IEEE, 2023, pp. 332–344.

