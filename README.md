# Jiatao Gu's thesis

# Title: Efficient Neural Machine Translation
# Abstract:
The dream of automatic translation that builds the communication bridge between people from different civilizations dates back to thousands of years ago. For the past decades, researchers devoted to proposing practical plans, from rule-based machine translation to statistical machine translation. In recent years, with the general success of artificial intelligence (AI) and the emergence of neural network models, a.k.a. deep learning, neural machine translation (NMT), as the new generation of machine translation framework based on sequence-to-sequence learning has achieved the state-of-the-art and even human-level translation performance on a variety of languages.

The impressive achievements brought by NMT are mainly due to its deep neural network structures with massive numbers of parameters, which can be efficiently tuned from vast volume of parallel data in the order of tens or hundreds of millions of sentences. Unfortunately, in spite of their success, neural systems also bring about new challenges to machine translation, in which one of the central problems is efficiency. The efficiency issue involves two aspects: 
(1) NMT is data-hungry because of its vast size of parameters, which makes training a reasonable model difficult in practice for low resource cases. For instance, most of the human languages do not have enough parallel data with other languages to learn an NMT model. Moreover, documents in specialized domains such as law or medicine usually contain tons of professional translations, leading to less efficiency for NMT to learn from;
(2) NMT is slow in computation compared to conventional methods due to its deep structure and limitations of the decoding algorithms. Especially the low efficiency at inference time profoundly affects the real-life application and the smoothness of the communication. In some cases like video conference, we also hope the neural system translates at real-time which, however, is difficult for the existing NMT models. 

This dissertation attempts to tackle these two challenges.
Contributions are twofold: 
(1) We address the data-efficiency challenges presented by existing NMT models and introduce insights based on the characteristics of the data, which includes 
(a) developing the copy-mechanism to target on rote memories in translation and general sequence-to-sequence learning; 
(b) using a non-parametric search-engine to guide the NMT system to perform well in special domains; 
(c) inventing a universal NMT system for extremely low resource languages; 
(d) extending the universal NMT system to be able to efficiently adapt to new languages by combing with meta-learning.

(2) For the decoding-efficiency challenges, we develop novel structures and learning algorithms, including
(a) recasting the decoding of NMT in a trainable manner to achieve state-of-the-art performance with less time; 
(b) inventing the non-autoregressive NMT system which enables translation in parallel; 
(c) developing the NMT model that learns to translate in real-time using reinforcement learning.
