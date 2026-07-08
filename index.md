---
layout: home
title: Home
---

# Neural networks that are both lean and fair

*Automatically designing neural architectures that are simultaneously frugal, hardware-adapted, and intrinsically free of algorithmic bias.*

This project is funded as an ANR JCJC (Jeunes Chercheuses et Jeunes Chercheurs) grant.

## Reconciling energy efficiency and algorithmic fairness in neural network design

Deep neural networks are growing increasingly complex, limiting their deployment on embedded devices and increasing their energy footprint. Current Neural Architecture Search (NAS) methods optimize generic criteria (FLOPs, memory) without accounting for either the target hardware or the presence of algorithmic bias — an issue that has become central with the entry into force of the EU AI Act, which mandates bias regulation even for compact architectures, a particularly fertile ground for bias to thrive. This project addresses this twofold gap by articulating computational sobriety and debiasing within a single design process.

## A three-pronged approach: measure, adapt, extract

**Measuring and limiting bias propagation.** Using tools from information theory, the project characterizes how bias propagates through networks' internal representations, and proposes differentiable terms that can be integrated into training to limit it (Barbano, Tartaglione & Grangetto, IEEE TAI 2024; Roos et al., WACV 2026).

**Designing hardware-aware penalty terms.** Architecture selection criteria sensitive to the target hardware (latency, caching, memory transfers) are developed to obtain compact, "green," transferable, and efficient models (Spadaro et al., Neurocomputing 2025; Olivi, Santero Mormile & Tartaglione, Scientific Reports 2025; Dalmasso et al., IJCNN 2025; Quétu et al., ICCV 2025; Wang et al., ICCV 2025).

**Searching for debiasing substructures.** The project demonstrates that unbiased subnetworks already pre-exist within conventionally trained models, and can be extracted without retraining or additional unbiased data (De Moura Matos et al., CVPR 2026).

## Results

The project has produced eight publications in leading international journals and conferences (CVPR, ICCV, WACV, IJCNN, IEEE TAI, Scientific Reports, Neurocomputing), covering all three axes of the project. The most striking result (De Moura Matos et al., CVPR 2026) establishes that a frugality/fairness trade-off is not antagonistic but complementary: structural pruning, a classic compression technique, can simultaneously reveal naturally less biased subnetworks, thereby validating the project's founding hypothesis that bias can be treated as a structural property of the architecture rather than merely an artifact of the data.

## Perspectives

This work paves the way for bias- and hardware-aware NAS methods capable of directly generating architectures compliant with regulatory requirements (AI Act) at no additional performance cost. Next steps aim to unify hardware sobriety and bias mitigation criteria within a single architecture search process, and to extend the BISE method to generative models (diffusion, multimodal LLMs), where bias amplification is particularly critical.

See the full list of results on the [Publications](publications.html) page.

{% include anr-ack.html %}
