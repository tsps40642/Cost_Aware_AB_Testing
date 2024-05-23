# Cost_Aware_AB_Testing

This is my project of Cost-Aware A/B Testing - Reinforcement learning and Causal Analysis.  
From UMN MSBA6461 Advanced AI for Business Applications.   

## Overview - Cost-Aware A/B Testing
A/B testing (a.k.a. randomized controlled trials, randomized experiments) is one of the most important ways to understand causal relationships. In a typical A/B testing setup, there will be one (or more) treatment group and one control group, and a pool of subjects are randomly assigned to the experimental groups based on pre-determined proportions (e.g., equal assignments).

While this is a perfectly legitimate way to test causality, it can be inefficient in practice. Imagine a clinical trial of two treatment options: drug A and placebo B, and let's assume that (in fact) drug A is much more effective than placebo B in treating a certain condition. Then, every subject that is assigned to the placebo group has to (unfortunately) endure some non-trivial costs, i.e., their conditions are not treated timely even when an effective drug exists. Note that some of the costs are necessary - after all, we don't know the effectiveness of drug A a priori and need a sufficient number of people in both groups to find out. However, as the effectiveness of drug A becomes clearer and clearer over the course of the experiment, perhaps it makes sense to gradually reduce the assignment to the placebo group, in order to reduce costs.

This is the basic idea behind cost-aware A/B testing. It is an important emerging topic in experimentation, and has attracted a lot of attention from both researchers and practitioners.

## Solution Overview - T-test for Causal Analysis 
My overall idea is to conduct T-test before assigning a treatment to a subject with a purpose to filter out the significantly inferior treatments, so that we won't assign those significantly inferior treatments to too many subjects after realizing their ineffectiveness.   

For more details, please refer to the Jupyter Notebook in the repository.  
