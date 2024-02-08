# Privacy Preserving Deep Learning Research List

This list provides up-to-date resources pertaining to the research and development of privacy-preserving deep learning, with many of them cited in the paper titled "[A Comprehensive Survey and Taxonomy on Privacy-Preserving Deep Learning](https://www.sciencedirect.com/science/article/abs/pii/S0925231224001164)". It will be consistently updated to reflect the latest findings and developments in the field of Privacy-Preserving Deep Learning (PPDL).

## Content
- [Privacy Leakages](#privacy-leakages)
- [Input Sharing](#input-sharing)
- [Model Sharing](#model-sharing)
- [Output Sharing](#output-sharing)
- [Libraries and Frameworks](#libraries-and-frameworks)


# Privacy Leakages

In the realm of machine learning, privacy leakages happen when flaws in models or systems unintentionally reveal confidential data of individuals involved in training or inference processes. These vulnerabilities can lead to various attacks like model inversion, membership inference, attribute inference, model extraction, and data poisoning, presenting risks such as privacy violations and discriminatory consequences. This section will outline cutting-edge attacks on deep learning models that result in privacy leakages.

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


