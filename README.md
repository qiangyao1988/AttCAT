<div align='center'>
 
# [AttCAT: Explaining Transformers via Attentive Class Activation Tokens](https://proceedings.neurips.cc/paper_files/paper/2022/file/20e45668fefa793bd9f2edf19be12c4b-Paper-Conference.pdf)

<table align="center">
  <tr>
    <td align="center"> 
      <img src="assets/methods.pdf" alt="Image 1" style="width: 700px;"/> 
      <br>
      <em style="font-size: 18px;">  <strong style="font-size: 18px;">Figure 1:</strong> A summary of the existing explanation methods and our methods.</em>
    </td>
  </tr>
</table>
</div>

Welcome to the official repository for the paper, [AttCAT: Explaining Transformers via Attentive Class Activation Tokens](https://proceedings.neurips.cc/paper_files/paper/2022/file/20e45668fefa793bd9f2edf19be12c4b-Paper-Conference.pdf). This repository contains the code for the experiments used in the paper.

## Abstract
Transformers have improved the state-of-the-art in various natural language processing and computer vision tasks. However, the success of the Transformer model has not yet been duly explained. Current explanation techniques, which dissect either the self-attention mechanism or gradient-based attribution, do not necessarily provide a faithful explanation of the inner workings of Transformers due to the following reasons: first, attention weights alone without considering the magnitudes of feature values are not adequate to reveal the self-attention mechanism; second, whereas most Transformer explanation techniques utilize self-attention module, the skip-connection module, contributing a significant portion of information flows in Transformers, has not yet been sufficiently exploited in explanation; third, the gradient-based attribution of individual feature does not incorporate interaction among features in explaining the model’s output. In order to tackle the above problems, we propose a novel Transformer explanation technique via attentive class activation tokens, aka, AttCAT, leveraging encoded features, their gradients, and their attention weights to generate a faithful and confident explanation for Transformer’s output. Extensive experiments are conducted to demonstrate the superior performance of AttCAT, which generalizes well to different Transformer architectures, evaluation metrics, datasets, and tasks, to the baseline methods

## Code structure
The code is structured as follows:
```
-- Run AttCAT and baseline methods for different datasets
    -- IMDB.ipynp
    -- MNLI.ipynp
    -- Yelp.ipynp
    -- QQP.ipynp
    -- SQUADv1/v2.ipynp
    -- SST-2.ipynp
-- Apply AttCAT to get heatmaps
    -- SST-2_Heatmap.ipynp
-- Get evaluations
    -- SST-2-Test.ipynp
```

## Cite This Work
```
@article{qiang2022attcat,
  title={Attcat: Explaining transformers via attentive class activation tokens},
  author={Qiang, Yao and Pan, Deng and Li, Chengyin and Li, Xin and Jang, Rhongho and Zhu, Dongxiao},
  journal={Advances in neural information processing systems},
  volume={35},
  pages={5052--5064},
  year={2022}
}
```
