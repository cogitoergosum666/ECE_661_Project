# ECE_661_Project
Chain of thought is all you need!


# GRPO Reasoning Alignment with Qwen2.5-3B

This project explores the use of **Group Relative Policy Optimization (GRPO)** to align the reasoning behavior of the Qwen2.5-3B language model. Our method fine-tunes the model via reinforcement learning using the **Unsloth** framework and **LoRA** adaptation, enabling efficient training on modest hardware.

### 🔍 Highlights
- **GRPO fine-tuning** enhances step-by-step reasoning capabilities without supervised reasoning traces.
- Achieves **83.67% accuracy on SVAMP**, outperforming much larger models.
- Shows improvements on **GSM8K** and reasoning-heavy MMLU subsets.
- Evaluates model alignment via custom control dimensions and structured prompts.

---

### 🗂 Repository Structure
- `Benchmark/`: Evaluation results on SVAMP, MMLU, SQuAD, and GSM8K.
- `Control Dimensions/`: Analysis of output consistency, reasoning structure, and failure cases.
- `Eval_Phi14b/`: Reference evaluation using a Phi-14B model for comparison.
- `README.md`: This file.
- `LICENSE`: MIT License.

---

### 🛠 Environment & Dependencies

You can reproduce our experiments using the following stack(to use unsloth you must use Linux env):

```bash
conda create -n grpo_qwen python=3.10
conda activate grpo_qwen

pip install torch transformers accelerate datasets
pip install peft unsloth vllm
```

### 📄 Citation
If you find this work helpful, please cite the poster:
> Haiwei Du, Linwei Wu, Yiran Wang. *Enhancing Reasoning Alignment in LLMs via GRPO Fine-Tuning: A Comparative Evaluation*. 2025.

---

For more information, refer to the poster or open an issue for questions.
