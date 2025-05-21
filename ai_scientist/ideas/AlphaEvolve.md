# Title: AlphaEvolve: Autonomous Evolutionary Code Synthesis with Gemini LLMs

## Keywords
algorithm discovery, evolutionary computation, large language models, code generation, automated evaluation

## TL;DR
AlphaEvolve combines Gemini-powered code generation, automated fitness evaluation, and evolutionary selection in a fully automated loop to discover novel, provably correct algorithms—surpassing decades-old human-designed baselines without manual prompt engineering.

## Abstract
We introduce AlphaEvolve, an end-to-end evolutionary coding agent that leverages state-of-the-art Gemini language models to autonomously discover and optimize algorithms at scale. 
Users provide a high-level code skeleton with designated evolution blocks and an executable fitness function. AlphaEvolve initializes a population of candidate implementations, then iterates through three core components: 
(1) a Prompt Sampler generates diverse child programs via LLM ensembles; 
(2) an Executable Evaluator runs and scores each variant on user-specified metrics; and 
(3) a Program Database retains top solutions to seed the next generation. 
This architecture scales to hundreds of lines of code in any programming language and operates fully automatically—eliminating manual prompt chaining or heuristics. 
We validate AlphaEvolve on both practical and theoretical tasks: optimizing Google’s data-center scheduling and hardware circuit routines, and advancing fundamental algorithmic benchmarks (e.g., discovering the first improvement to Strassen’s 4×4 matrix multiply in 56 years). 
Across 54 benchmark targets, AlphaEvolve matched or exceeded state-of-the-art bounds in 52 cases, demonstrating its ability to navigate vast search spaces and produce verifiable, high-performance code. 
By uniting LLM-driven proposal, rigorous automated evaluation, and evolutionary selection, AlphaEvolve paves the way for minimal-intervention algorithmic innovation in both applied and scientific domains.