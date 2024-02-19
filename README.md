<h1 align="center"><b>Privacy Preserving Deep Learning Research List</b></h1>
<p align="center">
    <a href="https://github.com/AndrewZhou924/Awesome-model-inversion-attack/pulls"><img src="https://img.shields.io/badge/PRs-Welcome-green" alt="PRs"></a>
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="awesome"></a>
</p>
This list provides up-to-date resources pertaining to the research and development of privacy-preserving deep learning, with many of them cited in the paper titled ["A Comprehensive Survey and Taxonomy on Privacy-Preserving Deep Learning"](https://www.sciencedirect.com/science/article/abs/pii/S0925231224001164). It will be consistently updated to reflect the latest findings and developments in the field of Privacy-Preserving Deep Learning (PPDL).  

![alt text](https://github.com/lab-secureai/Privacy-Preserving-Deep-Learning-Research-List/blob/main/img/ppdl1.JPG?raw=true)

**Please star or watch this repository to keep tracking the latest updates! Contributions are welcome!**

**Outlines:**
- [Surveys and Overviews](#survey-and-overviews)
- [Privacy Leakages](#privacy-leakages)
- [Input Sharing](#input-sharing)
- [Model Sharing](#model-sharing)
- [Output Sharing](#output-sharing)
- [Libraries and Frameworks](#libraries-and-frameworks)

# Surveys and Overviews

<!-- | Year | Title | Venue | Paper Link | Code Link |
| ---- | ----- | -------------------- | ----- | ---------- | --------- |

# Privacy Leakages

In the realm of machine learning, privacy leakages happen when flaws in models or systems unintentionally reveal confidential data of individuals involved in training or inference processes. These vulnerabilities can lead to various attacks like model inversion, membership inference, attribute inference, model extraction, and data poisoning, presenting risks such as privacy violations and discriminatory consequences. This section will outline cutting-edge attacks on deep learning models that result in privacy leakages.

## Model Inversion Attacks

<!-- | Year | Title | Adversarial Knowledge | Venue | Paper Link | Code Link |
| ---- | ----- | -------------------- | ----- | ---------- | --------- |
| 2014 | Privacy in pharmacogenetics: An end-to-end case study of personalized warfarin dosing | white-box | Security | [Paper](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf) | |
| 2015 | Model inversion attacks that exploit confidence information and basic countermeasures | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677) | [Code1](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip), [Code2](https://github.com/yashkant/Model-Inversion-Attack), [Code3](https://github.com/zhangzp9970/MIA), [Code4](https://github.com/sarahsimionescu/simple-model-inversion) |
| 2015 | Regression Model Fitting under Differential Privacy and Model Inversion Attack | | IJCAI | [Paper](http://www.csce.uark.edu/~xintaowu/publ/ijcai15.pdf) | [Code](https://github.com/cxs040/Regression-Model-Fitting-under-Differential-Privacy-and-Model-Inversion-Attack-Source-Code) |
| 2016 | A Methodology for Formalizing Model Inversion Attacks | | CSF | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL) | |
| 2017 | Machine Learning Models that Remember Too Much | | CCS | [Paper](https://arxiv.org/pdf/1709.07886.pdf) | [Code](https://github.com/csong27/ml-model-remember) |
| 2017 | Model inversion attacks for prediction systems: Without knowledge of non-sensitive attributes | | PST | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476925) | |
| 2018 | Privacy Risk in Machine Learning: Analyzing the Connection to Overfitting | | CSF | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429311) | |
| 2019 | MLPrivacyGuard: Defeating Confidence Information based Model Inversion Attacks on Machine Learning Systems | | GLSVLSI | [Paper](https://www.researchgate.net/profile/Tiago-Alves-13/publication/333136362_MLPrivacyGuard_Defeating_Confidence_Information_based_Model_Inversion_Attacks_on_Machine_Learning_Systems/links/5cddb94d92851c4eaba682d7/MLPrivacyGuard-Defeating_Confidence-Information-based-Model-Inversion-Attacks-on-Machine-Learning-Systems.pdf) | |
| 2019 | Model inversion attacks against collaborative inference | | ACSAC | [Paper](https://par.nsf.gov/servlets/purl/10208164) | [Code](https://github.com/zechenghe/Inverse_Collaborative_Inference) |
| 2019 | Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA) | [Code](https://github.com/zhangzp9970/TB-MIA) |
| 2019 | Exploiting Unintended Feature Leakage in Collaborative Learning | | S&P | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8835269) | [Code](https://github.com/csong27/property-inference-collaborative-ml) |
| 2019 | Adversarial Neural Network Inversion via Auxiliary Knowledge Alignment | | Arxiv | [Paper](https://arxiv.org/pdf/1902.08552.pdf) | |
| 2019 | GAMIN: An Adversarial Approach to Black-Box Model Inversion | | Arxiv | [Paper](https://arxiv.org/pdf/1909.11835.pdf) | |
| 2020 | The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks | white-box | CVPR | [Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf) | [Code](https://github.com/AI-secure/GMI-Attack), [Video](https://www.youtube.com/watch?v=_g-oXYMhz4M) |
| 2020 | Overlearning Reveals Sensitive Attributes | | ICLR | [Paper](https://arxiv.org/pdf/1905.11742.pdf) | |
| 2020 | Deep Face Recognizer Privacy Attack: Model Inversion Initialization by a Deep Generative Adversarial Data Space Discriminator | | APSIPA ASC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9306253&casa_token=AWugOvIe0I0AAAAA:9wICCkMcfoljMqooM-lgl8m-6F6-cEl-ClHgNkE1SV8mZwqvBIaJ1HDjT1RWLyBz_P7tdB51jQVL&tag=1) | |
| 2020 | Updates-Leak: Data Set Inference and Reconstruction Attacks in Online Learning | | USENIX Security | [Paper](https://www.usenix.org/system/files/sec20-salem.pdf) | |
| 2020 | Attacking and Protecting Data Privacy in Edge-Cloud Collaborative Inference Systems | | IoTJ | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9187880) | [Code](https://github.com/zechenghe/Inverse_Collaborative_Inference) |
| 2020 | Black-Box Face Recovery from Identity Features | | ECCV Workshop | [Paper](https://arxiv.org/pdf/2007.13635.pdf) | |
| 2020 | Defending model inversion and membership inference attacks via prediction purification | | Arxiv | [Paper](https://arxiv.org/pdf/2005.03915.pdf) | |
| 2020 | Generative model-inversion attacks against deep neural networks | white-box | CVPR | [Paper](https://arxiv.org/pdf/1911.07135.pdf) | [code](https://github.com/AI-secure/GMI-Attack) |
| 2020 | Privacy Preserving Facial Recognition Against Model Inversion Attacks | white-box | Globecom  | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9322508) |  |
| 2020 | Broadening Differential Privacy for Deep LearningAgainst Model Inversion Attacks  | white-box | Big Data | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9378274) |  |
| 2021 | Black-box adversarial attacks on commercial speech platforms with minimal information | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3460120.3485383) | |
| 2021 | Unleashing the tiger: Inference attacks on split learning | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3460120.3485259) | [Code](https://github.com/pasquini-dario/SplitNN_FSHA) |
| 2021 | Soteria: Provable defense against privacy leakage in federated learning from representation perspective | | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Sun_Soteria_Provable_Defense_Against_Privacy_Leakage_in_Federated_Learning_From_CVPR_2021_paper.pdf) | [Code](https://github.com/jeremy313/Soteria) |
| 2021 | Variational Model Inversion Attacks | | NeurIPS | [Paper](https://proceedings.neurips.cc/paper/2021/file/50a074e6a8da4662ae0a29edde722179-Paper.pdf) | [Code](https://github.com/wangkua1/vmi) |
| 2021 | Exploiting Explanations for Model Inversion Attacks | | ICCV | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_Exploiting_Explanations_for_Model_Inversion_Attacks_ICCV_2021_paper.pdf) | |
| 2021 | Knowledge-Enriched Distributional Model Inversion Attacks | | ICCV | [Paper](https://arxiv.org/pdf/2010.04092.pdf) | [Code](https://github.com/SCccc21/Knowledge-Enriched-DMI) |
| 2021 | Improving Robustness to Model Inversion Attacks via Mutual Information Regularization | | AAAI | [Paper](https://arxiv.org/pdf/2009.05241.pdf) | |
| 2021 | Practical Defences Against Model Inversion Attacks for Split Neural Networks | | ICLR Workshop | [Paper](https://arxiv.org/pdf/2104.05743.pdf) | [Code](https://github.com/TTitcombe/Model-Inversion-SplitNN), [Video](https://crossminds.ai/video/practical-defences-against-model-inversion-attacks-for-split-neural-networks-60c3cee46af07cfaf7325850/) |
| 2021 | Feature Inference Attack on Model Predictions in Vertical Federated Learning | | ICDE | [Paper](https://arxiv.org/pdf/2010.10152) | [Code](https://github.com/xj231/featureinference-vfl) |
| 2021 | PRID: Model Inversion Privacy Attacks in Hyperdimensional Learning Systems | | DAC | [Paper](https://dl.acm.org/doi/abs/10.1109/DAC18074.2021.9586217) | |
| 2021 | Robustness of On-Device Models: Adversarial Attack to Deep Learning Models on Android Apps | | ICSE | [Paper](https://arxiv.org/pdf/2101.04401) | |
| 2021 | Defending Against Model Inversion Attack by Adversarial Examples | | CSR Workshops | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9527945) | |
| 2021 | Practical Black Box Model Inversion Attacks Against Neural Nets | black-box | ECML PKDD | [Paper](https://link.springer.com/content/pdf/10.1007/978-3-030-93733-1.pdf?pdf=button) |  |
| 2021 | Model Inversion Attack against a Face Recognition System in a Black-Box Setting | black-box | APSIPA | [Paper](http://www.apsipa.org/proceedings/2021/pdfs/0001800.pdf) |  |
| 2022 | Plug & Play Attacks: Towards Robust and Flexible Model Inversion Attacks | | ICML | [Paper](https://arxiv.org/pdf/2201.12179.pdf) | [Code](https://github.com/LukasStruppek/Plug-and-Play-Attacks) |
| 2022 | Label-Only Model Inversion Attacks via Boundary Repulsion | | CVPR | [Paper](https://arxiv.org/pdf/2203.01925.pdf) | [Code](https://github.com/m-kahla/Label-Only-Model-Inversion-Attacks-via-Boundary-Repulsion) |
| 2022 | ResSFL: A Resistance Transfer Framework for Defending Model Inversion Attack in Split Federated Learning | | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Li_ResSFL_A_Resistance_Transfer_Framework_for_Defending_Model_Inversion_Attack_CVPR_2022_paper.html) | [Code](https://github.com/zlijingtao/ResSFL) |
| 2022 | Bilateral Dependency Optimization: Defending Against Model-Inversion Attacks | | KDD | [Paper](https://arxiv.org/pdf/2206.05483.pdf) | [Code](https://github.com/xpeng9719/Defend_MI) |
| 2022 | ML-DOCTOR: Holistic Risk Assessment of Inference Attacks Against Machine Learning Models | | USENIX Security | [Paper](https://www.usenix.org/system/files/sec22summer_liu-yugeng.pdf) | [Code](https://github.com/liuyugeng/ML-Doctor) |
| 2022 | An Approximate Memory Based Defense Against Model Inversion Attacks to Neural Networks | | IEEE | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9792582&casa_token=ymT57RhNhGEAAAAA:WsQHMpv77-4uyIp7l-p4hc7_Qmxvn5TeNpS5F7LHBFHyLay2O8Pe5eWqsKN2fu56v98NZsRrqeit) | [Code](https://github.com/katekemu/model_inversion_defense) |
| 2022 | Model Inversion Attack by Integration of Deep Generative Models: Privacy-Sensitive Face Generation From a Face Recognition System | | TIFS | [Paper](https://dl.acm.org/doi/abs/10.1109/TIFS.2022.3140687) | |
| 2022 | Defending Against Reconstruction Attacks Through Differentially Private Federated Learning for Classification of Heterogeneous Chest X-Ray Data | | Arxiv | [Paper](https://arxiv.org/pdf/2205.03168.pdf) | |
| 2022 | One Parameter Defense—Defending Against Data Inference Attacks via Differential Privacy | black-box | TIFS | [Paper](https://arxiv.org/pdf/2203.06580.pdf) |  |
| 2022 | Reconstructing Training Data from Diverse ML Models by Ensemble Inversion | white-box | WACV | [Paper](https://arxiv.org/pdf/2111.03702.pdf) |  |
| 2022 | SecretGen: Privacy Recovery on Pre-trained Models via Distribution Discrimination | white-box | ECCV | [Paper](https://arxiv.org/pdf/2207.12263.pdf) |  |
| 2022 | UnSplit: Data-Oblivious Model Inversion, Model Stealing, andLabel Inference Attacks Against Split Learning | S | WPES | [Paper](https://arxiv.org/pdf/2108.09033.pdf) | [code](https://github.com/ege-erdogan/unsplit) |
| 2022 | MIRROR: Model Inversion for Deep LearningNetwork with High Fidelity | white-box | NDSS | [Paper](https://www.cs.purdue.edu/homes/an93/static/papers/ndss2022_model_inversion.pdf) | [code](https://github.com/njuaplusplus/mirror) |
| 2023 | Sparse Black-Box Inversion Attack with Limited Information | black-box | ICASSP | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10095514) | [code](https://github.com/Tencent/TFace/tree/master/recognition) |
| 2023 | Breaching FedMD: Image Recovery via Paired-Logits Inversion Attack | black-box | CVPR | [Paper](https://arxiv.org/pdf/2304.11436.pdf) | [code](https://github.com/FLAIR-THU/PairedLogitsInversion) |
| 2023 | Pseudo Label-Guided Model Inversion Attack via Conditional Generative Adversarial Network | white-box | AAAI | [Paper](https://arxiv.org/pdf/2302.09814.pdf) | [code](https://github.com/lethesec/plg-mi-attack) |
| 2023 | C2FMI: Corse-to-Fine Black-box Model Inversion Attack | black-box | TDSC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148574) |  |
| 2023 | Boosting Model Inversion Attacks with Adversarial Examples | black-box | TDSC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148576) |  |
| 2023 | Reinforcement Learning-Based Black-Box Model Inversion Attacks | black-box | CVPR | [Paper](https://arxiv.org/pdf/2304.04625.pdf) | [code](https://github.com/HanGyojin/RLB-MI) |
| 2023 | Re-thinking Model Inversion Attacks Against Deep Neural Networks | white-box | CVPR | [Paper](https://arxiv.org/pdf/2304.01669.pdf) | [code](https://github.com/sutd-visual-computing-group/Re-thinking_MI) | -->

| Year | Title                                                        | Adversarial Knowledge | Venue           | Paper Link                                                   | Code Link                                                    |
| ---- | ------------------------------------------------------------ | --------------------- | --------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 2014 | Privacy in Pharmacogenetics: An End-to-End Case Study of Personalized Warfarin Dosing | white-box (both)      | USENIX Security | [paper](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf) |                                                              |
| 2015 | Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures | white-box (both)      | CCS             | [paper](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677)  | [code1](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip), [code2](https://github.com/yashkant/Model-Inversion-Attack), [code3](https://github.com/zhangzp9970/MIA), [code4](https://github.com/sarahsimionescu/simple-model-inversion) |
| 2015 | Regression model fitting under differential privacy and model inversion attack | white-box (defense)         | IJCAI           | [paper](http://www.csce.uark.edu/~xintaowu/publ/ijcai15.pdf) | [code](https://github.com/cxs040/Regression-Model-Fitting-under-Differential-Privacy-and-Model-Inversion-Attack-Source-Code) |
| 2016 | A Methodology for Formalizing Model-Inversion Attacks        | black & white-box             | CSF             | [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL) |                                                              |
| 2017 | Machine Learning Models that Remember Too Much               | white-box             | CCS             | [paper](https://arxiv.org/pdf/1709.07886.pdf)                | [code](https://github.com/csong27/ml-model-remember)         |
| 2017 | Model inversion attacks for prediction systems: Without knowledge of non-sensitive attributes | white-box             | PST             | [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476925) |                                                              |
| 2018 | Privacy Risk in Machine Learning: Analyzing the Connection to Overfitting | white-box | CSF | [paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429311) |     |
| 2019 | An Attack-Based Evaluation Method for Differentially Private Learning Against Model Inversion Attack | white-box  | arXiv   | [Paper](https://ieeexplore.ieee.org/document/8822435)      |  |
| 2019 | MLPrivacyGuard: Defeating Confidence Information based Model Inversion Attacks on Machine Learning Systems | black-box (defense)             | GLSVLSI         | [paper](https://www.researchgate.net/profile/Tiago-Alves-13/publication/333136362_MLPrivacyGuard_Defeating_Confidence_Information_based_Model_Inversion_Attacks_on_Machine_Learning_Systems/links/5cddb94d92851c4eaba682d7/MLPrivacyGuard-Defeating-Confidence-Information-based-Model-Inversion-Attacks-on-Machine-Learning-Systems.pdf) |                                                              |
| 2019 | Model inversion attacks against collaborative inference      | black & white-box (collaborative inference)           |         ACSAC        |    [Paper](http://palms.ee.princeton.edu/system/files/Model+Inversion+Attack+against+Collaborative+Inference.pdf)   |                                                              |
| 2019 | Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment | black-box | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA) | [Code](https://github.com/zhangzp9970/TB-MIA) | - |
| 2019 | GAMIN: An Adversarial Approach to Black-Box Model Inversion | black-box | Arxiv | [Paper](https://arxiv.org/pdf/1909.11835.pdf) | - | - |
| 2020 | The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks | white-box | CVPR | [Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf) | [Code](https://github.com/AI-secure/GMI-Attack) | [Video](https://www.youtube.com/watch?v=_g-oXYMhz4M) |
| 2020 | Overlearning Reveals Sensitive Attributes | white-box | ICLR | [Paper](https://arxiv.org/pdf/1905.11742.pdf) | - | - |
| 2020 | Deep Face Recognizer Privacy Attack: Model Inversion Initialization by a Deep Generative Adversarial Data Space Discriminator | white-box | APSIPA ASC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9306253&casa_token=AWugOvIe0I0AAAAA:9wICCkMcfoljMqooM-lgl8m-6F6-cEl-ClHgNkE1SV8mZwqvBIaJ1HDjT1RWLyBz_P7tdB51jQVL&tag=1) | - | - |
| 2020 | Updates-Leak: Data Set Inference and Reconstruction Attacks in Online Learning | black-box | USENIX Security | [Paper](https://www.usenix.org/system/files/sec20-salem.pdf) | - | - |
| 2020 | Attacking and Protecting Data Privacy in Edge-Cloud Collaborative Inference Systems | black-box (collaborative inference) | IoT-J | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9187880) | [Code](https://github.com/zechenghe/Inverse_Collaborative_Inference) | - |
| 2020 | Black-Box Face Recovery from Identity Features | black-box | ECCV Workshop | [Paper](https://arxiv.org/pdf/2007.13635.pdf) | - | - |
| 2020 | MixCon: Adjusting the Separability of Data Representations for Harder Data Recovery | white-box | arXiv  | [Paper](https://arxiv.org/abs/2010.11463) 
| 2020 | Privacy Preserving Facial Recognition Against Model Inversion Attacks | white-box (defense) | Globecom | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9322508) | - | - |
| 2020 | Broadening Differential Privacy for Deep Learning Against Model Inversion Attacks | white-box (defense) | Big Data | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9378274) | - | - |
| 2020 | Evaluation Indicator for Model Inversion Attack | metric | AdvML| [Paper](https://drive.google.com/file/d/1rl77BGtGHzZ8obWUEOoqunXCjgvpzE8d/view)   |                                                  |
| 2021 | Variational Model Inversion Attacks | white-box | NeurIPS | [Paper](https://proceedings.neurips.cc/paper/2021/file/50a074e6a8da4662ae0a29edde722179-Paper.pdf) | [Code](https://github.com/wangkua1/vmi) | - |
| 2021 | Exploiting Explanations for Model Inversion Attacks | white-box | ICCV | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_Exploiting_Explanations_for_Model_Inversion_Attacks_ICCV_2021_paper.pdf) | - |
| 2021 | Knowledge-Enriched Distributional Model Inversion Attacks | white-box | ICCV | [Paper](https://arxiv.org/pdf/2010.04092.pdf) | [Code](https://github.com/SCccc21/Knowledge-Enriched-DMI) |
| 2021 | Improving Robustness to Model Inversion Attacks via Mutual Information Regularization | white-box (defense) | AAAI | [Paper](https://arxiv.org/pdf/2009.05241.pdf) | - |
| 2021 | Practical Defences Against Model Inversion Attacks for Split Neural Networks | black-box (defense, collaborative inference) | ICLR workshop | [Paper](https://arxiv.org/pdf/2104.05743.pdf) | [Code](https://github.com/TTitcombe/Model-Inversion-SplitNN) |
| 2021 | Feature inference attack on model predictions in vertical federated learning | white-box (VFL) | ICDE | [Paper](https://arxiv.org/pdf/2010.10152) | [Code](https://github.com/xj231/featureinference-vfl) |
| 2021 | PRID: Model Inversion Privacy Attacks in Hyperdimensional Learning Systems | black-box (both, collaborative inference) | DAC | [Paper](https://dl.acm.org/doi/abs/10.1109/DAC18074.2021.9586217) | - |
| 2021 | Defending Against Model Inversion Attack by Adversarial Examples | black-box (defense) | CSR Workshops | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9527945) | - |
| 2021 | Practical Black Box Model Inversion Attacks Against Neural Nets | black-box | ECML PKDD | [Paper](https://link.springer.com/chapter/10.1007/978-3-030-93733-1_3) | - |
| 2021 | Model Inversion Attack against a Face Recognition System in a Black-Box Setting | black-box | APSIPA | [Paper](http://www.apsipa.org/proceedings/2021/pdfs/0001800.pdf) | - |
| 2022 | Plug & Play Attacks: Towards Robust and Flexible Model Inversion Attacks | white-box | ICML | [Paper](https://arxiv.org/pdf/2201.12179.pdf) | [Code](https://github.com/LukasStruppek/Plug-and-Play-Attacks) |
| 2022 | Label-Only Model Inversion Attacks via Boundary Repulsion | black-box | CVPR | [Paper](https://arxiv.org/pdf/2203.01925.pdf) | [Code](https://github.com/m-kahla/Label-Only-Model-Inversion-Attacks-via-Boundary-Repulsion) |
| 2022 | ResSFL: A Resistance Transfer Framework for Defending Model Inversion Attack in Split Federated Learning | white-box (defense, SFL) | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Li_ResSFL_A_Resistance_Transfer_Framework_for_Defending_Model_Inversion_Attack_CVPR_2022_paper.html) | [Code](https://github.com/zlijingtao/ResSFL) |
| 2022 | Bilateral Dependency Optimization: Defending Against Model-inversion Attacks | white-box (defense) | KDD | [Paper](https://arxiv.org/pdf/2206.05483.pdf) | [Code](https://github.com/xpeng9719/Defend_MI) |
| 2022 | ML-DOCTOR: Holistic Risk Assessment of Inference Attacks Against Machine Learning Models | holistic risk assessment | USENIX Security | [Paper](https://www.usenix.org/system/files/sec22summer_liu-yugeng.pdf) | [Code](https://github.com/liuyugeng/ML-Doctor) |
| 2022 | Model Inversion Attack by Integration of Deep Generative Models: Privacy-Sensitive Face Generation From a Face Recognition System | white-box | TIFS | [Paper](https://dl.acm.org/doi/abs/10.1109/TIFS.2022.3140687) | - |
| 2022 | One Parameter Defense—Defending Against Data Inference Attacks via Differential Privacy | black-box (defense) | TIFS | [Paper](https://arxiv.org/pdf/2203.06580.pdf) |  |
| 2022 | Reconstructing Training Data from Diverse ML Models by Ensemble Inversion | white-box | WACV | [Paper](https://arxiv.org/pdf/2111.03702.pdf) |  |
| 2022 | SecretGen: Privacy Recovery on Pre-trained Models via Distribution Discrimination | white-box | ECCV | [Paper](https://arxiv.org/pdf/2207.12263.pdf) |  |
| 2022 | UnSplit: Data-Oblivious Model Inversion, Model Stealing, and Label Inference Attacks Against Split Learning | black-box (split learnig) | WPES | [Paper](https://arxiv.org/pdf/2108.09033.pdf) | [code](https://github.com/ege-erdogan/unsplit) |
| 2022 | MIRROR: Model Inversion for Deep LearningNetwork with High Fidelity | white-box | NDSS | [Paper](https://www.cs.purdue.edu/homes/an93/static/papers/ndss2022_model_inversion.pdf) | [code](https://github.com/njuaplusplus/mirror) |
| 2022 | Reconstructing Training Data with Informed Adversaries | white-box  | SP | [Paper](https://arxiv.org/abs/2201.04845)   |           |
| 2022 | Privacy Vulnerability of Split Computing to Data-Free Model Inversion Attacks  | white-box | BMVC | [Paper](https://arxiv.org/abs/2107.06304)   
| 2022 | Reconstructing Training Data from Trained Neural Networks | white-box  | NeurIPS   | [Paper](https://arxiv.org/abs/2206.07758)     |                                                             |
| 2023 | Sparse Black-Box Inversion Attack with Limited Information | black-box | ICASSP | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10095514) | [code](https://github.com/Tencent/TFace/tree/master/recognition) |
| 2023 | Breaching FedMD: Image Recovery via Paired-Logits Inversion Attack | black-box | CVPR | [Paper](https://arxiv.org/pdf/2304.11436.pdf) | [code](https://github.com/FLAIR-THU/PairedLogitsInversion) |
| 2023 | Pseudo Label-Guided Model Inversion Attack via Conditional Generative Adversarial Network | white-box | AAAI | [Paper](https://arxiv.org/pdf/2302.09814.pdf) | [code](https://github.com/lethesec/plg-mi-attack) |
| 2023 | C2FMI: Corse-to-Fine Black-box Model Inversion Attack | black-box | TDSC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148574) |  |
| 2023 | Boosting Model Inversion Attacks with Adversarial Examples | black-box | TDSC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148576) |  |
| 2023 | Reinforcement Learning-Based Black-Box Model Inversion Attacks | black-box | CVPR | [Paper](https://arxiv.org/pdf/2304.04625.pdf) | [code](https://github.com/HanGyojin/RLB-MI) |
| 2023 | Re-thinking Model Inversion Attacks Against Deep Neural Networks | white-box | CVPR | [Paper](https://arxiv.org/pdf/2304.01669.pdf) | [code](https://github.com/sutd-visual-computing-group/Re-thinking_MI) |
| 2023 | Purifier: Defending Data Inference Attacks via Transforming Confidence Scores | black-box (defense) | AAAI | [Paper](https://arxiv.org/pdf/2005.03915.pdf) | - | - |
| 2023 | Unstoppable Attack: Label-Only Model Inversion via Conditional Diffusion Model | black-box | CCS | [Paper](https://arxiv.org/pdf/2307.08424.pdf) | - | - |


# Input Sharing

In this setup, a service provider server handles both model training and deployment. User data undergo various protection methods like Secure Multiparty Computation (SMC), Homomorphic Encryption (HE), etc., before being transferred to the server. All training and prediction occur centrally on the server. Centralized learning offers several advantages:
- It reduces client computation resources, requiring only transformed data sharing.
- It supports collaboration in an unstable network environment.
- It allows for operations on non-identically distributed data (non-iid).
- It efficiently handles models with minimal data, such as fully distributed data models.
- It enables constructing versatile models from shared data for various purposes.

Due to these benefits, centralized learning has garnered significant attention. Original data are transformed using HE algorithms, SMC protocols, secret sharing techniques, or noise addition before sharing with the server. These data transformation methods can be categorized in three main techniques: cryptography-based, data obfuscation, and secure enclaves-based techniques.

## Cryptography-based methods

## Data obfuscation methods

## Other methods

# Model Sharing

# Output Sharing

# Libraries and Frameworks


