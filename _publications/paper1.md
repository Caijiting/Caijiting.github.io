---
title: "Take A Step Back: Rethinking the Two Stages in Visual Reasoning"
collection: publications
category: conferences
permalink: /publication/paper1
date: 2024-07-01
venue: 'ECCV 2024'
paperurl: 'https://arxiv.org/pdf/2407.19666v1'
---

Visual reasoning, as a prominent research area, plays a crucial role in AI by facilitating concept formation and interaction with the world. However, current works are usually carried out separately on small datasets thus lacking generalization ability. Through rigorous evaluation of diverse benchmarks, we demonstrate the shortcomings of existing methods in achieving cross-domain reasoning and their tendency to data bias fitting. In this paper, we revisit visual reasoning with a two-stage perspective: (1) symbolization and (2) logical reasoning given symbols or their representations. We find that the reasoning stage is better at generalization than symbolization. Thus, it is more efficient to implement symbolization via separated encoders for different data domains while using a shared reasoner. Given our findings, we establish design principles for visual reasoning frameworks following the separated symbolization and shared reasoning. Our two-stage framework achieves impressive generalization ability on various visual reasoning tasks, including puzzles, physical prediction, and visual question answering (VQA), encompassing both 2D and 3D modalities. We believe our insights will pave the way for generalizable visual reasoning. Our code will be publicly available.
