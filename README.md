<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🌋 LLaVA：大型语言和视觉助手</font></font></h1><a id="user-content--llava-large-language-and-vision-assistant" class="anchor" aria-label="永久链接：🌋 LLaVA：大型语言和视觉助手" href="#-llava-large-language-and-vision-assistant"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">针对具有 GPT-4 级别功能的大型语言和视觉模型进行视觉指令调整。</font></font></em></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[📢 </font></font><a href="https://llava-vl.github.io/blog/2024-01-30-llava-next/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-NeXT 博客</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://llava-vl.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目页面</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://llava.hliu.cc/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Data.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型动物园</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🤝社区贡献：[ </font></font><a href="https://github.com/ggerganov/llama.cpp/pull/3436" data-hovercard-type="pull_request" data-hovercard-url="/ggerganov/llama.cpp/pull/3436/hovercard"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">llama.cpp</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ] [ </font></font><a href="https://github.com/camenduru/LLaVA-colab"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Colab</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ] [ </font></font><a href="https://huggingface.co/spaces/badayvedat/LLaVA" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🤗Space</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ] [</font></font><a href="https://replicate.com/yorickvp/llava-13b" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">复制</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [ </font></font><a href="https://github.com/microsoft/autogen/blob/main/notebook/agentchat_lmm_llava.ipynb"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">AutoGen</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ] [ </font></font><a href="https://github.com/SkunkworksAI/BakLLaVA"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BakLLaVA</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ]</font></font></p>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">通过视觉指令调整改进基线</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[</font></font><a href="https://arxiv.org/abs/2310.03744" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">论文</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [ </font></font><a href="https://huggingface.co/papers/2310.03744" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">HF</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ] </font></font><br>
<a href="https://hliu.cc" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Haotian Liu</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> , </font></font><a href="https://chunyuan.li/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Chunyuan Li</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> , </font></font><a href="https://yuheng-li.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Yuheng Li</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> , </font></font><a href="https://pages.cs.wisc.edu/~yongjaelee/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Yong Jae Lee</font></font></a></p>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视觉指令调优</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（NeurIPS 2023，</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">口头</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）[</font></font><a href="https://arxiv.org/abs/2304.08485" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">论文</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">][</font></font><a href="https://huggingface.co/papers/2304.08485" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">高频</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] </font></font><br>
<a href="https://hliu.cc" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Haotian Liu*</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font><a href="https://chunyuan.li/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Chunyuan Li*</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font><a href="https://scholar.google.ca/citations?user=HDiw-TsAAAAJ&amp;hl=en/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Qingyang Wu</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font><a href="https://pages.cs.wisc.edu/~yongjaelee/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Yong Jae Lee</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（*同等贡献）</font></font></p>

<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布</font></font></h2><a id="user-content-release" class="anchor" aria-label="永久链接：发布" href="#release"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[2024/05/10] 🔥 </font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-NeXT</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> (Stronger) 模型发布，更强的 LMM，支持 LLama-3 (8B) 和 Qwen-1.5 (72B/110B)。 [</font></font><a href="https://llava-vl.github.io/blog/2024-05-10-llava-next-stronger-llms/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">博客</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://huggingface.co/collections/lmms-lab/llava-next-6623288e2d61edba3ddbf5ff" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">检查点</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://llava-next.lmms-lab.com/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/LLaVA-VL/LLaVA-NeXT/"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[2024/05/10] 🔥 </font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-NeXT</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">（视频）发布。仅图像训练的 LLaVA-NeXT 模型在零样本模态传输的视频任务上出奇地强大。通过视频的 AI 反馈进行 DPO 培训可以带来显着的改进。 [</font></font><a href="https://llava-vl.github.io/blog/2024-04-30-llava-next-video/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">博客</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://huggingface.co/collections/lmms-lab/llava-next-video-661e86f5e8dabc3ff793c944" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">检查点</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/LLaVA-VL/LLaVA-NeXT/"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[03/10] 发布</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LMMs-Eval</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，这是我们在开发 LLaVA-NeXT 时使用的高效评估流程。它支持在数十个公共数据集上评估 LMM，并允许新数据集加入，从而使新 LMM 的开发速度更快。 [</font></font><a href="https://lmms-lab.github.io/lmms-eval-blog/lmms-eval-0.1/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">博客</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/EvolvingLMMs-Lab/lmms-eval"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码库</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[1/30] 🔥 </font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-NeXT</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> (LLaVA-1.6) 出炉了！通过额外扩展到 LLaVA-1.5，LLaVA-NeXT-34B 在某些基准测试中优于 Gemini Pro。它现在可以处理比以前多 4 倍的像素并执行更多的任务/应用程序。查看</font></font><a href="https://llava-vl.github.io/blog/2024-01-30-llava-next/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">博客文章</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并探索</font></font><a href="https://llava.hliu.cc/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">！模型可在</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Model Zoo</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中找到。培训/评估数据和脚本即将推出。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[11/10] </font></font><a href="https://llava-vl.github.io/llava-plus/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-Plus</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布：学习使用用于创建多模式代理的工具，带有 LLaVA-Plus（LLaVA 即插即用学习使用技能）。 [</font></font><a href="https://llava-vl.github.io/llava-plus/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目页面</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://llavaplus.ngrok.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/LLaVA-VL/LLaVA-Plus-Codebase"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://arxiv.org/abs/2311.05437" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">论文</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[11/2] </font></font><a href="https://llava-vl.github.io/llava-interactive/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-Interactive</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布：通过图像聊天、分割、生成和编辑的一体化演示体验人机交互的未来。 [</font></font><a href="https://llava-vl.github.io/llava-interactive/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目页面</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://llavainteractive.ngrok.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://github.com/LLaVA-VL/LLaVA-Interactive-Demo"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">代码</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">] [</font></font><a href="https://arxiv.org/abs/2311.00571" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">论文</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[10/26] 🔥 采用 LoRA 的 LLaVA-1.5 实现了与全模型微调相当的性能，同时降低了 GPU RAM 要求（</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md#llava-v15"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">ckpts</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://github.com/haotian-liu/LLaVA#train"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">脚本</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）。我们还提供了</font><font style="vertical-align: inherit;">有关如何使用 LoRA 在您自己的数据集上微调 LLaVA-1.5 的</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Finetune_Custom_Data.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">文档。</font></font></a><font style="vertical-align: inherit;"></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[10/12] 看看由ETRI创建的韩国LLaVA（Ko-LLaVA），ETRI慷慨支持我们的研究！ [ </font></font><a href="https://huggingface.co/spaces/etri-vilab/Ko-LLaVA" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">🤗 演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[10/5] 🔥 LLaVA-1.5 出炉了！只需对原始 LLaVA 进行简单修改，即可在 11 个基准上实现 SoTA，利用所有公共数据，在单个 8-A100 节点上约 1 天完成训练，超越 Qwen-VL-Chat 等使用十亿级数据的方法。查看</font></font><a href="https://arxiv.org/abs/2310.03744" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">技术报告</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">并探索</font></font><a href="https://llava.hliu.cc/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">！模型可在</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Model Zoo</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中找到。 LLaVA-1.5的训练数据和脚本</font></font><a href="https://github.com/haotian-liu/LLaVA#train"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这里</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布，评估脚本</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Evaluation.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这里</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">发布</font><font style="vertical-align: inherit;">！</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[9/26] LLaVA 通过人类反馈的强化学习 (RLHF) 进行了改进，以改善事实基础并减少幻觉。查看项目</font></font><a href="https://llava-rlhf.github.io/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[LLavA-RLHF]中的新 SFT 和 RLHF 检查点</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">[9/22] </font></font><a href="https://arxiv.org/abs/2304.08485" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">被 NeurIPS 2023 接受为</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">口头报告</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font><a href="https://arxiv.org/abs/2306.00890" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-Med</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">被 NeurIPS 2023 数据集和基准跟踪接受为</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">聚光报告</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
</ul>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">更多的</font></font></summary>
<ul dir="auto">
<li>[11/6] Support <strong>Intel</strong> dGPU and CPU platforms. <a href="https://github.com/haotian-liu/LLaVA/tree/intel/docs/intel">More details here.</a></li>
<li>[10/12] LLaVA is now supported in <a href="https://github.com/ggerganov/llama.cpp/pull/3436" data-hovercard-type="pull_request" data-hovercard-url="/ggerganov/llama.cpp/pull/3436/hovercard">llama.cpp</a> with 4-bit / 5-bit quantization support!</li>
<li>[10/11] The training data and scripts of LLaVA-1.5 are released <a href="https://github.com/haotian-liu/LLaVA#train">here</a>, and evaluation scripts are released <a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Evaluation.md">here</a>!</li>
<li>[10/10] <a href="https://blog.roboflow.com/first-impressions-with-llava-1-5/" rel="nofollow">Roboflow Deep Dive</a>: First Impressions with LLaVA-1.5.</li>
<li>[9/20] We summarize our empirical study of training 33B and 65B LLaVA models in a <a href="https://arxiv.org/abs/2309.09958" rel="nofollow">note</a>. Further, if you are interested in the comprehensive review, evolution and trend of multimodal foundation models, please check out our recent survey paper <a href="https://arxiv.org/abs/2309.10020" rel="nofollow">``Multimodal Foundation Models: From Specialists to General-Purpose Assistants''.</a></li>
</ul>
<p align="center" dir="auto">
  <a target="_blank" rel="noopener noreferrer" href="https://github.com/Computer-Vision-in-the-Wild/CVinW_Readings/blob/main/images/mfm_evolution.jpeg?raw=true"><img src="https://github.com/Computer-Vision-in-the-Wild/CVinW_Readings/raw/main/images/mfm_evolution.jpeg?raw=true" width="50%/" style="max-width: 100%;"></a>
</p>
<ul dir="auto">
<li>[7/19] 🔥 We release a major upgrade, including support for LLaMA-2, LoRA training, 4-/8-bit inference, higher resolution (336x336), and a lot more. We release <a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/LLaVA_Bench.md">LLaVA Bench</a> for benchmarking open-ended visual chat with results from Bard and Bing-Chat. We also support and verify training with RTX 3090 and RTX A6000. Check out <a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/LLaVA_from_LLaMA2.md">LLaVA-from-LLaMA-2</a>, and our <a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md">model zoo</a>!</li>
<li>[6/26] <a href="https://vlp-tutorial.github.io/" rel="nofollow">CVPR 2023 Tutorial</a> on <strong>Large Multimodal Models: Towards Building and Surpassing Multimodal GPT-4</strong>!  Please check out [<a href="https://datarelease.blob.core.windows.net/tutorial/vision_foundation_models_2023/slides/Chunyuan_cvpr2023_tutorial_lmm.pdf" rel="nofollow">Slides</a>] [<a href="https://arxiv.org/abs/2306.14895" rel="nofollow">Notes</a>] [<a href="https://youtu.be/mkI7EPD1vp8" rel="nofollow">YouTube</a>] [<a href="https://www.bilibili.com/video/BV1Ng4y1T7v3/" rel="nofollow">Bilibli</a>].</li>
<li>[6/11] We released the preview for the most requested feature: DeepSpeed and LoRA support!  Please see documentations <a href="/haotian-liu/LLaVA/blob/main/docs/LoRA.md">here</a>.</li>
<li>[6/1] We released <strong>LLaVA-Med: Large Language and Vision Assistant for Biomedicine</strong>, a step towards building biomedical domain large language and vision models with GPT-4 level capabilities.  Checkout the <a href="https://arxiv.org/abs/2306.00890" rel="nofollow">paper</a> and <a href="https://github.com/microsoft/LLaVA-Med">page</a>.</li>
<li>[5/6] We are releasing <a href="https://huggingface.co/liuhaotian/LLaVA-Lightning-MPT-7B-preview" rel="nofollow">LLaVA-Lighting-MPT-7B-preview</a>, based on MPT-7B-Chat!  See <a href="#LLaVA-MPT-7b">here</a> for more details.</li>
<li>[5/2] 🔥 We are releasing LLaVA-Lighting!  Train a lite, multimodal GPT-4 with just $40 in 3 hours!  See <a href="#train-llava-lightning">here</a> for more details.</li>
<li>[4/27] Thanks to the community effort, LLaVA-13B with 4-bit quantization allows you to run on a GPU with as few as 12GB VRAM!  Try it out <a href="https://github.com/oobabooga/text-generation-webui/tree/main/extensions/llava">here</a>.</li>
<li>[4/17] 🔥 We released <strong>LLaVA: Large Language and Vision Assistant</strong>. We propose visual instruction tuning, towards building large language and vision models with GPT-4 level capabilities.  Checkout the <a href="https://arxiv.org/abs/2304.08485" rel="nofollow">paper</a> and <a href="https://llava.hliu.cc/" rel="nofollow">demo</a>.</li>
</ul>
</details>

<p dir="auto"><a href="https://github.com/tatsu-lab/stanford_alpaca/blob/main/LICENSE"><img src="https://camo.githubusercontent.com/ff42248868bc1387751598955e573b397851d947f13ddd7618c0ba9e66aacdf6/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f436f64652532304c6963656e73652d4170616368655f322e302d677265656e2e737667" alt="代码许可" data-canonical-src="https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg" style="max-width: 100%;"></a>
<strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用和许可声明</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：该项目使用某些数据集和检查点，这些数据集和检查点受各自原始许可的约束。用户必须遵守这些原始许可证的所有条款和条件，包括但不限于数据集的</font></font><a href="https://openai.com/policies/terms-of-use" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OpenAI 使用条款</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以及使用数据集训练的检查点的基本语言模型的特定许可证（例如</font><font style="vertical-align: inherit;">Llama-2 的</font></font><a href="https://ai.meta.com/llama/license/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Llama 社区许可证</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和骆驼毛-v1.5)。除了原始许可证中规定的限制外，该项目没有施加任何额外的限制。此外，提醒用户确保他们对数据集和检查点的使用符合所有适用的法律和法规。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">内容</font></font></h2><a id="user-content-contents" class="anchor" aria-label="永久链接： 内容" href="#contents"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="#install"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装</font></font></a></li>
<li><a href="#llava-weights"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA 权重</font></font></a></li>
<li><a href="#Demo"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></a></li>
<li><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型动物园</font></font></a></li>
<li><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Data.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据集</font></font></a></li>
<li><a href="#train"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">火车</font></font></a></li>
<li><a href="#evaluation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">评估</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装</font></font></h2><a id="user-content-install" class="anchor" aria-label="永久链接：安装" href="#install"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您使用的不是 Linux，请</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不要继续，请参阅</font></font></em><font style="vertical-align: inherit;"></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/macOS.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">macOS</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Windows.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Windows</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的说明</font><font style="vertical-align: inherit;">。</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">克隆此存储库并导航到 LLaVA 文件夹</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>git clone https://github.com/haotian-liu/LLaVA.git
<span class="pl-c1">cd</span> LLaVA</pre><div class="zeroclipboard-container">
     
  </div></div>
<ol start="2" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">安装包</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>conda create -n llava python=3.10 -y
conda activate llava
pip install --upgrade pip  <span class="pl-c"><span class="pl-c">#</span> enable PEP 660 support</span>
pip install -e <span class="pl-c1">.</span></pre><div class="zeroclipboard-container">
    
  </div></div>
<ol start="3" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为培训案例安装附加包</font></font></li>
</ol>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>pip install -e ".[train]"
pip install flash-attn --no-build-isolation
</code></pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">升级到最新的代码库</font></font></h3><a id="user-content-upgrade-to-latest-code-base" class="anchor" aria-label="永久链接：升级到最新的代码库" href="#upgrade-to-latest-code-base"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>git pull
pip install -e <span class="pl-c1">.</span>

<span class="pl-c"><span class="pl-c">#</span> if you see some import errors when you upgrade,</span>
<span class="pl-c"><span class="pl-c">#</span> please try running the command below (without #)</span>
<span class="pl-c"><span class="pl-c">#</span> pip install flash-attn --no-build-isolation --no-cache-dir</span></pre><div class="zeroclipboard-container">
   
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">快速开始使用 HuggingFace</font></font></h3><a id="user-content-quick-start-with-huggingface" class="anchor" aria-label="永久链接：HuggingFace 快速入门" href="#quick-start-with-huggingface"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">示例代码</font></font></summary>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">from</span> <span class="pl-s1">llava</span>.<span class="pl-s1">model</span>.<span class="pl-s1">builder</span> <span class="pl-k">import</span> <span class="pl-s1">load_pretrained_model</span>
<span class="pl-k">from</span> <span class="pl-s1">llava</span>.<span class="pl-s1">mm_utils</span> <span class="pl-k">import</span> <span class="pl-s1">get_model_name_from_path</span>
<span class="pl-k">from</span> <span class="pl-s1">llava</span>.<span class="pl-s1">eval</span>.<span class="pl-s1">run_llava</span> <span class="pl-k">import</span> <span class="pl-s1">eval_model</span>

<span class="pl-s1">model_path</span> <span class="pl-c1">=</span> <span class="pl-s">"liuhaotian/llava-v1.5-7b"</span>

<span class="pl-s1">tokenizer</span>, <span class="pl-s1">model</span>, <span class="pl-s1">image_processor</span>, <span class="pl-s1">context_len</span> <span class="pl-c1">=</span> <span class="pl-en">load_pretrained_model</span>(
    <span class="pl-s1">model_path</span><span class="pl-c1">=</span><span class="pl-s1">model_path</span>,
    <span class="pl-s1">model_base</span><span class="pl-c1">=</span><span class="pl-c1">None</span>,
    <span class="pl-s1">model_name</span><span class="pl-c1">=</span><span class="pl-en">get_model_name_from_path</span>(<span class="pl-s1">model_path</span>)
)</pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto">Check out the details wth the <code>load_pretrained_model</code> function in <code>llava/model/builder.py</code>.</p>
<p dir="auto">You can also use the <code>eval_model</code> function in <code>llava/eval/run_llava.py</code> to get the output easily. By doing so, you can use this code on Colab directly after downloading this repository.</p>
<div class="highlight highlight-source-python notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-s1">model_path</span> <span class="pl-c1">=</span> <span class="pl-s">"liuhaotian/llava-v1.5-7b"</span>
<span class="pl-s1">prompt</span> <span class="pl-c1">=</span> <span class="pl-s">"What are the things I should be cautious about when I visit here?"</span>
<span class="pl-s1">image_file</span> <span class="pl-c1">=</span> <span class="pl-s">"https://llava-vl.github.io/static/images/view.jpg"</span>

<span class="pl-s1">args</span> <span class="pl-c1">=</span> <span class="pl-en">type</span>(<span class="pl-s">'Args'</span>, (), {
    <span class="pl-s">"model_path"</span>: <span class="pl-s1">model_path</span>,
    <span class="pl-s">"model_base"</span>: <span class="pl-c1">None</span>,
    <span class="pl-s">"model_name"</span>: <span class="pl-en">get_model_name_from_path</span>(<span class="pl-s1">model_path</span>),
    <span class="pl-s">"query"</span>: <span class="pl-s1">prompt</span>,
    <span class="pl-s">"conv_mode"</span>: <span class="pl-c1">None</span>,
    <span class="pl-s">"image_file"</span>: <span class="pl-s1">image_file</span>,
    <span class="pl-s">"sep"</span>: <span class="pl-s">","</span>,
    <span class="pl-s">"temperature"</span>: <span class="pl-c1">0</span>,
    <span class="pl-s">"top_p"</span>: <span class="pl-c1">None</span>,
    <span class="pl-s">"num_beams"</span>: <span class="pl-c1">1</span>,
    <span class="pl-s">"max_new_tokens"</span>: <span class="pl-c1">512</span>
})()

<span class="pl-en">eval_model</span>(<span class="pl-s1">args</span>)</pre><div class="zeroclipboard-container">
     
  </div></div>
</details>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA 权重</font></font></h2><a id="user-content-llava-weights" class="anchor" aria-label="永久链接：LLaVA 权重" href="#llava-weights"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请查看我们的</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型动物园</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，了解所有公共 LLaVA 检查点以及如何使用权重的说明。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">演示</font></font></h2><a id="user-content-demo" class="anchor" aria-label="永久链接：演示" href="#demo"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">渐变网页用户界面</font></font></h3><a id="user-content-gradio-web-ui" class="anchor" aria-label="永久链接：Gradio Web UI" href="#gradio-web-ui"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要在本地启动 Gradio 演示，请一一运行以下命令。如果您计划启动多个模型工作人员以在不同检查点之间进行比较，则只需启动控制器和 Web 服务器</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">一次</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<section class="js-render-needs-enrichment render-needs-enrichment position-relative" data-identity="28e855c8-9ee8-424f-b6ec-973764bea271" data-host="https://viewscreen.githubusercontent.com" data-src="https://viewscreen.githubusercontent.com/markdown/mermaid?docs_host=https%3A%2F%2Fdocs.github.com" data-type="mermaid" aria-label="美人鱼渲染的输出容器">
  <div class="js-render-enrichment-target" data-json="{&quot;data&quot;:&quot;flowchart BT\n    %% Declare Nodes\n    gws(\&quot;Gradio (UI Server)\&quot;)\n    c(\&quot;Controller (API Server):&amp;lt;br/&amp;gt;PORT: 10000\&quot;)\n    mw7b(\&quot;Model Worker:&amp;lt;br/&amp;gt;llava-v1.5-7b&amp;lt;br/&amp;gt;PORT: 40000\&quot;)\n    mw13b(\&quot;Model Worker:&amp;lt;br/&amp;gt;llava-v1.5-13b&amp;lt;br/&amp;gt;PORT: 40001\&quot;)\n    sglw13b(\&quot;SGLang Backend:&amp;lt;br/&amp;gt;llava-v1.6-34b&amp;lt;br/&amp;gt;http://localhost:30000\&quot;)\n    lsglw13b(\&quot;SGLang Worker:&amp;lt;br/&amp;gt;llava-v1.6-34b&amp;lt;br/&amp;gt;PORT: 40002\&quot;)\n\n    %% Declare Styles\n    classDef data fill:#3af,stroke:#48a,stroke-width:2px,color:#444\n    classDef success fill:#8f8,stroke:#0a0,stroke-width:2px,color:#444\n    classDef failure fill:#f88,stroke:#f00,stroke-width:2px,color:#444\n\n    %% Assign Styles\n    class id,od data;\n    class cimg,cs_s,scsim_s success;\n    class ncimg,cs_f,scsim_f failure;\n\n    subgraph Demo Connections\n        direction BT\n        c&amp;lt;--&amp;gt;gws\n        \n        mw7b&amp;lt;--&amp;gt;c\n        mw13b&amp;lt;--&amp;gt;c\n        lsglw13b&amp;lt;--&amp;gt;c\n        sglw13b&amp;lt;--&amp;gt;lsglw13b\n    end\n&quot;}" data-plain="flowchart BT
    %% Declare Nodes
    gws(&quot;Gradio (UI Server)&quot;)
    c(&quot;Controller (API Server):<br/>PORT: 10000&quot;)
    mw7b(&quot;Model Worker:<br/>llava-v1.5-7b<br/>PORT: 40000&quot;)
    mw13b(&quot;Model Worker:<br/>llava-v1.5-13b<br/>PORT: 40001&quot;)
    sglw13b(&quot;SGLang Backend:<br/>llava-v1.6-34b<br/>http://localhost:30000&quot;)
    lsglw13b(&quot;SGLang Worker:<br/>llava-v1.6-34b<br/>PORT: 40002&quot;)

    %% Declare Styles
    classDef data fill:#3af,stroke:#48a,stroke-width:2px,color:#444
    classDef success fill:#8f8,stroke:#0a0,stroke-width:2px,color:#444
    classDef failure fill:#f88,stroke:#f00,stroke-width:2px,color:#444

    %% Assign Styles
    class id,od data;
    class cimg,cs_s,scsim_s success;
    class ncimg,cs_f,scsim_f failure;

    subgraph Demo Connections
        direction BT
        c<-->gws
        
        mw7b<-->c
        mw13b<-->c
        lsglw13b<-->c
        sglw13b<-->lsglw13b
    end
" dir="auto"><!----><!----><div class="position-absolute top-0 pr-2 right-0 d-flex flex-justify-end flex-items-center">
    
    <details class="details-reset details-overlay details-overlay-dark" style="display: contents">
      <summary role="button" aria-label="打开对话框" class="btn my-2 mr-2 p-0 d-inline-flex" aria-haspopup="dialog">
        <svg width="16" height="16" viewBox="0 0 16 16" fill="currentColor" class="octicon m-2">
          <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 1.06L2.56 7h10.88l-2.22-2.22a.75.75 0 011.06-1.06l3.5 3.5a.75.75 0 010 1.06l-3.5 3.5a.75.75 0 11-1.06-1.06l2.22-2.22H2.56l2.22 2.22a.75.75 0 11-1.06 1.06l-3.5-3.5a.75.75 0 010-1.06l3.5-3.5z"></path>
        </svg>
      </summary>
      <details-dialog class="Box Box--overlay render-full-screen d-flex flex-column anim-fade-in fast" aria-label="mermaid rendered container" role="dialog" aria-modal="true">
        <div>
          <button aria-label="Close dialog" data-close-dialog="" type="button" data-view-component="true" class="Link--muted btn-link position-absolute render-full-screen-close">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="display:inline-block;vertical-align:text-bottom" class="octicon octicon-x">
              <path fill-rule="evenodd" d="M5.72 5.72a.75.75 0 011.06 0L12 10.94l5.22-5.22a.75.75 0 111.06 1.06L13.06 12l5.22 5.22a.75.75 0 11-1.06 1.06L12 13.06l-5.22 5.22a.75.75 0 01-1.06-1.06L10.94 12 5.72 6.78a.75.75 0 010-1.06z"></path>
            </svg>
          </button>
          <div class="Box-body border-0" role="presentation"></div>
        </div>
      </details-dialog>
    </details>
  <!----> 
  </div><!---->
    <div class="render-container color-bg-transparent js-render-target p-0 is-render-automatic is-render-requested is-render-ready" data-identity="28e855c8-9ee8-424f-b6ec-973764bea271" data-host="https://viewscreen.githubusercontent.com" data-type="mermaid" style="height: 396.225px;">
       
    </div>
  <!----><!----></div>
  <span class="js-render-enrichment-loader d-flex flex-justify-center flex-items-center width-full" style="min-height:100px" role="presentation" hidden="">
    <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" data-view-component="true" class="octospinner mx-auto anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" fill="none"></circle>
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke"></path>
</svg>
  </span>
<div class="js-render-enrichment-fallback"><div class="render-plaintext-hidden" dir="auto">
      <pre lang="mermaid" aria-label="Raw mermaid code">flowchart BT
    %% Declare Nodes
    gws("Gradio (UI Server)")
    c("Controller (API Server):&lt;br/&gt;PORT: 10000")
    mw7b("Model Worker:&lt;br/&gt;llava-v1.5-7b&lt;br/&gt;PORT: 40000")
    mw13b("Model Worker:&lt;br/&gt;llava-v1.5-13b&lt;br/&gt;PORT: 40001")
    sglw13b("SGLang Backend:&lt;br/&gt;llava-v1.6-34b&lt;br/&gt;http://localhost:30000")
    lsglw13b("SGLang Worker:&lt;br/&gt;llava-v1.6-34b&lt;br/&gt;PORT: 40002")

    %% Declare Styles
    classDef data fill:#3af,stroke:#48a,stroke-width:2px,color:#444
    classDef success fill:#8f8,stroke:#0a0,stroke-width:2px,color:#444
    classDef failure fill:#f88,stroke:#f00,stroke-width:2px,color:#444

    %% Assign Styles
    class id,od data;
    class cimg,cs_s,scsim_s success;
    class ncimg,cs_f,scsim_f failure;

    subgraph Demo Connections
        direction BT
        c&lt;--&gt;gws
        
        mw7b&lt;--&gt;c
        mw13b&lt;--&gt;c
        lsglw13b&lt;--&gt;c
        sglw13b&lt;--&gt;lsglw13b
    end
</pre>
    </div></div></section>

<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动控制器</font></font></h4><a id="user-content-launch-a-controller" class="anchor" aria-label="永久链接：启动控制器" href="#launch-a-controller"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.controller --host 0.0.0.0 --port 10000</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动 gradio Web 服务器。</font></font></h4><a id="user-content-launch-a-gradio-web-server" class="anchor" aria-label="永久链接：启动 gradio Web 服务器。" href="#launch-a-gradio-web-server"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.gradio_web_server --controller http://localhost:10000 --model-list-mode reload</pre><div class="zeroclipboard-container">
   
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您刚刚启动了 Gradio Web 界面。现在，您可以打开 Web 界面，并将 URL 打印在屏幕上。您可能会注意到模型列表中没有模型。别担心，我们还没有推出任何劳模。当您启动模型工作人员时，它将自动更新。</font></font></p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动 SGLang 工作线程</font></font></h4><a id="user-content-launch-a-sglang-worker" class="anchor" aria-label="永久链接：启动 SGLang 工作线程" href="#launch-a-sglang-worker"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这是高吞吐量服务 LLaVA 模型的推荐方式，您需要先安装 SGLang。请注意，目前</font></font><code>4-bit</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">SGLang-LLaVA 尚不支持量化，如果您的 GPU VRAM 有限，请查看带有</font></font><a href="https://github.com/haotian-liu/LLaVA?tab=readme-ov-file#launch-a-model-worker-4-bit-8-bit-inference-quantized"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">量化</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">的模型工作器。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>pip install <span class="pl-s"><span class="pl-pds">"</span>sglang[all]<span class="pl-pds">"</span></span></pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您将首先启动 SGLang 后端工作程序，它将在 GPU 上执行模型。记住</font></font><code>--port</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您设置的，稍后您将使用它。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c"><span class="pl-c">#</span> Single GPU</span>
CUDA_VISIBLE_DEVICES=0 python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --port 30000

<span class="pl-c"><span class="pl-c">#</span> Multiple GPUs with tensor parallel</span>
CUDA_VISIBLE_DEVICES=0,1 python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-13b --tokenizer-path llava-hf/llava-1.5-13b-hf --port 30000 --tp 2</pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">分词器（临时）：</font></font><code>llava-hf/llava-1.5-7b-hf</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">, </font></font><code>llava-hf/llava-1.5-13b-hf</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">, </font></font><code>liuhaotian/llava-v1.6-34b-tokenizer</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">然后，您将启动一个 LLaVA-SGLang 工作程序，它将在 LLaVA 控制器和 SGLang 后端之间进行通信以路由请求。设置</font></font><code>--sgl-endpoint</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为</font><font style="vertical-align: inherit;">您刚刚设置的位置（默认值：30000）</font></font><code>http://127.0.0.1:port</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font><code>port</code><font style="vertical-align: inherit;"></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.sglang_worker --host 0.0.0.0 --controller http://localhost:10000 --port 40000 --worker http://localhost:40000 --sgl-endpoint http://127.0.0.1:30000</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开展劳动模范活动</font></font></h4><a id="user-content-launch-a-model-worker" class="anchor" aria-label="永久链接：启动模范工人" href="#launch-a-model-worker"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这是</font><font style="vertical-align: inherit;">在 GPU 上执行推理的实际</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">工作程序</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。每个工作人员负责 中指定的单个模型</font></font><code>--model-path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.model_worker --host 0.0.0.0 --controller http://localhost:10000 --port 40000 --worker http://localhost:40000 --model-path liuhaotian/llava-v1.5-13b</pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">等到进程完成加载模型，您会看到“Uvicorn running on ...”。现在，刷新您的 Gradio Web UI，您将在模型列表中看到刚刚启动的模型。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以根据需要启动任意数量的工作程序，并在同一 Gradio 界面中比较不同模型检查点。请保持</font></font><code>--controller</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">不变，并将 和 修改</font></font><code>--port</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为</font></font><code>--worker</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">每个worker的不同端口号。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.model_worker --host 0.0.0.0 --controller http://localhost:10000 --port <span class="pl-k">&lt;</span>different from 40000, say <span class="pl-k">40001&gt;</span> --worker http://localhost:<span class="pl-k">&lt;</span>change accordingly, i.e. <span class="pl-k">40001&gt;</span> --model-path <span class="pl-k">&lt;</span>ckpt<span class="pl-k">2&gt;</span></pre><div class="zeroclipboard-container">
    
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您使用的是带有 M1 或 M2 芯片的 Apple 设备，则可以使用标志指定 mps 设备</font></font><code>--device</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：</font></font><code>--device mps</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动模型工作人员（多个 GPU，当 GPU VRAM &lt;= 24GB 时）</font></font></h4><a id="user-content-launch-a-model-worker-multiple-gpus-when-gpu-vram--24gb" class="anchor" aria-label="永久链接：启动模型工作线程（多个 GPU，当 GPU VRAM <= 24GB 时）" href="#launch-a-model-worker-multiple-gpus-when-gpu-vram--24gb"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您的 GPU 的 VRAM 小于 24GB（例如 RTX 3090、RTX 4090 等），您可以尝试使用多个 GPU 运行它。如果您有多个 GPU，我们最新的代码库将自动尝试使用多个 GPU。您可以指定要使用哪些 GPU </font></font><code>CUDA_VISIBLE_DEVICES</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。下面是使用前两个 GPU 运行的示例。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>CUDA_VISIBLE_DEVICES=0,1 python -m llava.serve.model_worker --host 0.0.0.0 --controller http://localhost:10000 --port 40000 --worker http://localhost:40000 --model-path liuhaotian/llava-v1.5-13b</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动模型工作者（4位、8位推理、量化）</font></font></h4><a id="user-content-launch-a-model-worker-4-bit-8-bit-inference-quantized" class="anchor" aria-label="永久链接：启动模型工作者（4 位、8 位推理、量化）" href="#launch-a-model-worker-4-bit-8-bit-inference-quantized"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以使用量化位（4 位、8 位）启动模型工作线程，这样您就可以在减少 GPU 内存占用的情况下运行推理，从而有可能在具有低至 12GB VRAM 的 GPU 上运行。请注意，使用量化位进行的推理可能不如全精度模型准确。只需将</font></font><code>--load-4bit</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">或附加</font></font><code>--load-8bit</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">到</font><font style="vertical-align: inherit;">您正在执行的</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型工作器</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">命令即可。下面是使用 4 位量化运行的示例。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.model_worker --host 0.0.0.0 --controller http://localhost:10000 --port 40000 --worker http://localhost:40000 --model-path liuhaotian/llava-v1.5-13b --load-4bit</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">启动模型工作者（LoRA 权重，未合并）</font></font></h4><a id="user-content-launch-a-model-worker-lora-weights-unmerged" class="anchor" aria-label="永久链接：启动模型工作者（LoRA 权重，未合并）" href="#launch-a-model-worker-lora-weights-unmerged"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以启动具有 LoRA 权重的模型工作线程，无需将它们与基本检查点合并，以节省磁盘空间。会有额外的加载时间，而推理速度与合并检查点相同。未合并的 LoRA 检查点在型号名称中没有</font></font><code>lora-merge</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，并且通常比合并的检查点小得多（小于 1GB）（7B 为 13G，13B 为 25G）。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要加载未合并的 LoRA 权重，您只需传递一个附加参数</font></font><code>--model-base</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，它是用于训练 LoRA 权重的基础 LLM。您可以在</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">模型动物园</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">中检查每个 LoRA 权重的基础 LLM </font><font style="vertical-align: inherit;">。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.model_worker --host 0.0.0.0 --controller http://localhost:10000 --port 40000 --worker http://localhost:40000 --model-path liuhaotian/llava-v1-0719-336px-lora-vicuna-13b-v1.3 --model-base lmsys/vicuna-13b-v1.3</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CLI 推理</font></font></h3><a id="user-content-cli-inference" class="anchor" aria-label="永久链接：CLI 推理" href="#cli-inference"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 LLaVA 讨论图像，无需 Gradio 界面。它还支持多个 GPU、4 位和 8 位量化推理。通过 4 位量化，对于我们的 LLaVA-1.5-7B，它在单个 GPU 上使用不到 8GB VRAM。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python -m llava.serve.cli \
    --model-path liuhaotian/llava-v1.5-7b \
    --image-file <span class="pl-s"><span class="pl-pds">"</span>https://llava-vl.github.io/static/images/view.jpg<span class="pl-pds">"</span></span> \
    --load-4bit</pre><div class="zeroclipboard-container">
     
  </div></div>
<p dir="auto"><animated-image data-catalyst="" style="width: 70%;"><a target="_blank" rel="noopener noreferrer" href="/haotian-liu/LLaVA/blob/main/images/demo_cli.gif" data-target="animated-image.originalLink" hidden=""><img src="/haotian-liu/LLaVA/raw/main/images/demo_cli.gif" style="max-width: 100%;" data-target="animated-image.originalImage" hidden=""></a>
      <span class="AnimatedImagePlayer" data-target="animated-image.player">
        <a data-target="animated-image.replacedLink" class="AnimatedImagePlayer-images" href="https://github.com/haotian-liu/LLaVA/blob/main/images/demo_cli.gif" target="_blank">
          <span data-target="animated-image.imageContainer">
            <img data-target="animated-image.replacedImage" alt="" class="AnimatedImagePlayer-animatedImage" src="https://github.com/haotian-liu/LLaVA/raw/main/images/demo_cli.gif">
          </span>
        </a>
        <button data-target="animated-image.imageButton" class="AnimatedImagePlayer-images" tabindex="-1"></button>
        <span class="AnimatedImagePlayer-controls" data-target="animated-image.controls">
          <button data-target="animated-image.playButton" class="AnimatedImagePlayer-button">
            <svg aria-hidden="true" focusable="false" class="octicon icon-play" width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M4 13.5427V2.45734C4 1.82607 4.69692 1.4435 5.2295 1.78241L13.9394 7.32507C14.4334 7.63943 14.4334 8.36057 13.9394 8.67493L5.2295 14.2176C4.69692 14.5565 4 14.1739 4 13.5427Z">
            </path></svg>
            <svg aria-hidden="true" focusable="false" class="octicon icon-pause" width="16" height="16" viewBox="0 0 16 16" xmlns="http://www.w3.org/2000/svg">
              <rect x="4" y="2" width="3" height="12" rx="1"></rect>
              <rect x="9" y="2" width="3" height="12" rx="1"></rect>
            </svg>
          </button>
          <a data-target="animated-image.openButton" aria-label="Open in new window" class="AnimatedImagePlayer-button" href="https://github.com/haotian-liu/LLaVA/blob/main/images/demo_cli.gif" target="_blank">
            <svg aria-hidden="true" class="octicon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 16 16" width="16" height="16">
              <path fill-rule="evenodd" d="M10.604 1h4.146a.25.25 0 01.25.25v4.146a.25.25 0 01-.427.177L13.03 4.03 9.28 7.78a.75.75 0 01-1.06-1.06l3.75-3.75-1.543-1.543A.25.25 0 0110.604 1zM3.75 2A1.75 1.75 0 002 3.75v8.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 12.25v-3.5a.75.75 0 00-1.5 0v3.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-8.5a.25.25 0 01.25-.25h3.5a.75.75 0 000-1.5h-3.5z"></path>
            </svg>
          </a>
        </span>
      </span></animated-image></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">火车</font></font></h2><a id="user-content-train" class="anchor" aria-label="永久链接： 火车" href="#train"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">以下是 LLaVA v1.5 的最新训练配置。对于旧模型，请</font><font style="vertical-align: inherit;">暂时</font><font style="vertical-align: inherit;">参考</font></font><a href="https://github.com/haotian-liu/LLaVA/tree/v1.0.1"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">该</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">版本的README。稍后我们会将它们添加到单独的文档中。</font></font></em></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA 训练由两个阶段组成：（1）特征对齐阶段：使用我们的 LAION-CC-SBU 数据集的 558K 子集将</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">冻结的预训练</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视觉编码器连接到</font></font><em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">冻结的 LLM</font></font></em><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">； (2) 视觉指令调优阶段：使用 150K GPT 生成的多模态指令跟踪数据，加上来自学术导向任务的约 515K VQA 数据，来教导模型遵循多模态指令。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA 在 8 个具有 80GB 内存的 A100 GPU 上进行训练。要在更少的 GPU 上进行训练，您可以相应地减少</font></font><code>per_device_train_batch_size</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和增加</font></font><code>gradient_accumulation_steps</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。始终保持全局批量大小相同：</font></font><code>per_device_train_batch_size</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">x </font></font><code>gradient_accumulation_steps</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">x </font></font><code>num_gpus</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">超参数</font></font></h3><a id="user-content-hyperparameters" class="anchor" aria-label="永久链接：超参数" href="#hyperparameters"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们在微调中使用了一组与 Vicuna 类似的超参数。下面提供了预训练和微调中使用的两个超参数。</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">预训练</font></font></li>
</ol>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">超参数</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">全局批量大小</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">学习率</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">纪元</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最长长度</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">重量衰减</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-v1.5-13B</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">256</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">1e-3</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">1</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2048</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">0</font></font></td>
</tr>
</tbody>
</table>
<ol start="2" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">微调</font></font></li>
</ol>
<table>
<thead>
<tr>
<th><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">超参数</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">全局批量大小</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">学习率</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">纪元</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">最长长度</font></font></th>
<th align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">重量衰减</font></font></th>
</tr>
</thead>
<tbody>
<tr>
<td><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-v1.5-13B</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">128</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2e-5</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">1</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">2048</font></font></td>
<td align="right"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">0</font></font></td>
</tr>
</tbody>
</table>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载 Vicuna 检查点（自动）</font></font></h3><a id="user-content-download-vicuna-checkpoints-automatically" class="anchor" aria-label="永久链接：下载 Vicuna 检查点（自动）" href="#download-vicuna-checkpoints-automatically"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们的基本模型 Vicuna v1.5 是一个经过指令调整的聊天机器人，当您运行我们提供的训练脚本时，将会自动下载。无需采取任何行动。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">预训练（特征对齐）</font></font></h3><a id="user-content-pretrain-feature-alignment" class="anchor" aria-label="永久链接：预训练（特征对齐）" href="#pretrain-feature-alignment"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请下载 LAION-CC-SBU 数据集的 558K 子集，其中包含我们在本文中使用的 BLIP</font></font><a href="https://huggingface.co/datasets/liuhaotian/LLaVA-Pretrain" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">字幕</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">由于分辨率增加至 336px，LLaVA-v1.5-13B 在 8x A100 (80G) 上的预训练大约需要 5.5 小时。 LLaVA-v1.5-7B 大约需要 3.5 小时。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 DeepSpeed ZeRO-2 的训练脚本：</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/scripts/v1_5/pretrain.sh"><code>pretrain.sh</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></p>
<ul dir="auto">
<li><code>--mm_projector_type mlp2x_gelu</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：两层 MLP 视觉语言连接器。</font></font></li>
<li><code>--vision_tower openai/clip-vit-large-patch14-336</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：剪辑 ViT-L/14 336px。</font></font></li>
</ul>
<details>
<summary><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-7B 在 8x V100 (32G) 上的预训练大约需要 20 小时</font></font></summary>
<p dir="auto">We provide training script with DeepSpeed <a href="https://github.com/haotian-liu/LLaVA/blob/main/scripts/pretrain_xformers.sh">here</a>.
Tips:</p>
<ul dir="auto">
<li>If you are using V100 which is not supported by FlashAttention, you can use the <a href="https://arxiv.org/abs/2112.05682" rel="nofollow">memory-efficient attention</a> implemented in <a href="https://github.com/facebookresearch/xformers">xFormers</a>. Install xformers and replace <code>llava/train/train_mem.py</code> above with <a href="/haotian-liu/LLaVA/blob/main/llava/train/train_xformers.py">llava/train/train_xformers.py</a>.</li>
</ul>
</details>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视觉指令调整</font></font></h3><a id="user-content-visual-instruction-tuning" class="anchor" aria-label="永久链接：视觉指令调整" href="#visual-instruction-tuning"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备数据</font></font></li>
</ol>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请下载最终混合物的注释我们的指令调整数据</font></font><a href="https://huggingface.co/datasets/liuhaotian/LLaVA-Instruct-150K/blob/main/llava_v1_5_mix665k.json" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">llava_v1_5_mix665k.json</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，并从构成数据集中下载图像：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">可可：</font></font><a href="http://images.cocodataset.org/zips/train2017.zip" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">火车2017</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GQA：</font></font><a href="https://downloads.cs.stanford.edu/nlp/data/gqa/images.zip" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">图像</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">OCR-VQA：</font></font><a href="https://drive.google.com/drive/folders/1_GYPY5UkUy7HIcR0zq3ZCFgeZN7BAfm_?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载脚本</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们将所有文件保存为</font></font><code>.jpg</code></strong></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">TextVQA：</font></font><a href="https://dl.fbaipublicfiles.com/textvqa/images/train_val_images.zip" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">train_val_images</font></font></a></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">视觉基因组：</font></font><a href="https://cs.stanford.edu/people/rak248/VG_100K_2/images.zip" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">第 1 部分</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><a href="https://cs.stanford.edu/people/rak248/VG_100K_2/images2.zip" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">第 2 部分</font></font></a></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载完所有数据后，按如下方式组织数据</font></font><code>./playground/data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>├── coco
│   └── train2017
├── gqa
│   └── images
├── ocr_vqa
│   └── images
├── textvqa
│   └── train_images
└── vg
    ├── VG_100K
    └── VG_100K_2
</code></pre><div class="zeroclipboard-container">
   
  </div></div>
<ol start="2" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">开始训练！</font></font></li>
</ol>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以在</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/MODEL_ZOO.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Model Zoo</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载我们预先训练的投影仪。不建议使用旧版投影仪，因为它们可能使用不同版本的代码库进行训练，如果关闭任何选项，模型将无法按我们的预期运行/训练。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">由于分辨率增加至 336px，LLaVA-v1.5-13B 在 8x A100 (80G) 上的视觉指令调整大约需要 20 小时。 LLaVA-v1.5-7B 在 8x A100 (40G) 上大约需要 10 小时。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 DeepSpeed ZeRO-3 的训练脚本：</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/scripts/v1_5/finetune.sh"><code>finetune.sh</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">.</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您没有足够的 GPU 内存：</font></font></p>
<ul dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用LoRA </font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/scripts/v1_5/finetune_lora.sh"><code>finetune_lora.sh</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：.我们能够在 8-A100-40G/8-A6000 中进行 13B 训练，在 8-RTX3090 中进行 7B 训练。确保</font></font><code>per_device_train_batch_size*gradient_accumulation_steps</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">与提供的脚本相同以获得最佳重现性。</font></font></li>
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">替换</font></font><code>zero3.json</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为</font></font><code>zero3_offload.json</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">将某些参数卸载到 CPU RAM。这会减慢训练速度。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您有兴趣根据自己的任务/数据微调 LLaVA 模型，请查看</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Finetune_Custom_Data.md"><code>Finetune_Custom_Data.md</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">需要注意的新选项：</font></font></p>
<ul dir="auto">
<li><code>--mm_projector_type mlp2x_gelu</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：两层 MLP 视觉语言连接器。</font></font></li>
<li><code>--vision_tower openai/clip-vit-large-patch14-336</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：剪辑 ViT-L/14 336px。</font></font></li>
<li><code>--image_aspect_ratio pad</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：这会将非方形图像填充为方形，而不是裁剪它们；它会稍微减少幻觉。</font></font></li>
<li><code>--group_by_modality_length True</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：仅当您的指令调整数据集同时包含语言（例如 ShareGPT）和多模式（例如 LLaVA-Instruct）时才应使用此选项。它使训练采样器在训练期间仅采样单一模态（图像或语言），我们观察到这可以将训练速度加快约 25%，并且不会影响最终结果。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">评估</font></font></h2><a id="user-content-evaluation" class="anchor" aria-label="永久链接：评估" href="#evaluation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在 LLaVA-1.5 中，我们根据 12 个不同的基准来评估模型。为了确保可重复性，我们用贪婪解码来评估模型。我们不评估使用波束搜索使推理过程与实时输出的聊天演示一致。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请参阅</font></font><a href="https://github.com/haotian-liu/LLaVA/blob/main/docs/Evaluation.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">评估.md</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">GPT辅助评估</font></font></h3><a id="user-content-gpt-assisted-evaluation" class="anchor" aria-label="永久链接：GPT 辅助评估" href="#gpt-assisted-evaluation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们提供用于多模态建模的 GPT 辅助评估管道，以便全面了解视觉语言模型的功能。请参阅我们的论文了解更多详细信息。</font></font></p>
<ol dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">生成 LLaVA 响应</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python model_vqa.py \
    --model-path ./checkpoints/LLaVA-13B-v0 \
    --question-file \
    playground/data/coco2014_val_qa_eval/qa90_questions.jsonl \
    --image-folder \
    /path/to/coco2014_val \
    --answers-file \
    /path/to/answer-file-our.jsonl</pre><div class="zeroclipboard-container">
     
  </div></div>
<ol start="2" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">评估生成的响应。在我们的例子中，</font></font><a href="/haotian-liu/LLaVA/blob/main/playground/data/coco2014_val_qa_eval/qa90_gpt4_answer.jsonl"><code>answer-file-ref.jsonl</code></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是由纯文本 GPT-4 (0314) 生成的响应，并提供了上下文标题/框。</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>OPENAI_API_KEY=<span class="pl-s"><span class="pl-pds">"</span>sk-***********************************<span class="pl-pds">"</span></span> python llava/eval/eval_gpt_review_visual.py \
    --question playground/data/coco2014_val_qa_eval/qa90_questions.jsonl \
    --context llava/eval/table/caps_boxes_coco2014_val_80.jsonl \
    --answer-list \
    /path/to/answer-file-ref.jsonl \
    /path/to/answer-file-our.jsonl \
    --rule llava/eval/table/rule.json \
    --output /path/to/review.json</pre><div class="zeroclipboard-container">
    
  </div></div>
<ol start="3" dir="auto">
<li><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">总结评估结果</font></font></li>
</ol>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python summarize_gpt_review.py</pre><div class="zeroclipboard-container">
    
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引文</font></font></h2><a id="user-content-citation" class="anchor" aria-label="永久链接：引文" href="#citation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您发现 LLaVA 对您的研究和应用有用，请使用此 BibTeX 进行引用：</font></font></p>
<div class="highlight highlight-text-bibtex notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">@misc</span>{<span class="pl-en">liu2024llavanext</span>,
    <span class="pl-s">title</span>=<span class="pl-s"><span class="pl-pds">{</span>LLaVA-NeXT: Improved reasoning, OCR, and world knowledge<span class="pl-pds">}</span></span>,
    <span class="pl-s">url</span>=<span class="pl-s"><span class="pl-pds">{</span>https://llava-vl.github.io/blog/2024-01-30-llava-next/<span class="pl-pds">}</span></span>,
    <span class="pl-s">author</span>=<span class="pl-s"><span class="pl-pds">{</span>Liu, Haotian and Li, Chunyuan and Li, Yuheng and Li, Bo and Zhang, Yuanhan and Shen, Sheng and Lee, Yong Jae<span class="pl-pds">}</span></span>,
    <span class="pl-s">month</span>=<span class="pl-s"><span class="pl-pds">{</span>January<span class="pl-pds">}</span></span>,
    <span class="pl-s">year</span>=<span class="pl-s"><span class="pl-pds">{</span>2024<span class="pl-pds">}</span></span>
}

<span class="pl-k">@misc</span>{<span class="pl-en">liu2023improvedllava</span>,
      <span class="pl-s">title</span>=<span class="pl-s"><span class="pl-pds">{</span>Improved Baselines with Visual Instruction Tuning<span class="pl-pds">}</span></span>, 
      <span class="pl-s">author</span>=<span class="pl-s"><span class="pl-pds">{</span>Liu, Haotian and Li, Chunyuan and Li, Yuheng and Lee, Yong Jae<span class="pl-pds">}</span></span>,
      <span class="pl-s">publisher</span>=<span class="pl-s"><span class="pl-pds">{</span>arXiv:2310.03744<span class="pl-pds">}</span></span>,
      <span class="pl-s">year</span>=<span class="pl-s"><span class="pl-pds">{</span>2023<span class="pl-pds">}</span></span>,
}

<span class="pl-k">@misc</span>{<span class="pl-en">liu2023llava</span>,
      <span class="pl-s">title</span>=<span class="pl-s"><span class="pl-pds">{</span>Visual Instruction Tuning<span class="pl-pds">}</span></span>, 
      <span class="pl-s">author</span>=<span class="pl-s"><span class="pl-pds">{</span>Liu, Haotian and Li, Chunyuan and Wu, Qingyang and Lee, Yong Jae<span class="pl-pds">}</span></span>,
      <span class="pl-s">publisher</span>=<span class="pl-s"><span class="pl-pds">{</span>NeurIPS<span class="pl-pds">}</span></span>,
      <span class="pl-s">year</span>=<span class="pl-s"><span class="pl-pds">{</span>2023<span class="pl-pds">}</span></span>,
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@misc{liu2024llavanext,
    title={LLaVA-NeXT: Improved reasoning, OCR, and world knowledge},
    url={https://llava-vl.github.io/blog/2024-01-30-llava-next/},
    author={Liu, Haotian and Li, Chunyuan and Li, Yuheng and Li, Bo and Zhang, Yuanhan and Shen, Sheng and Lee, Yong Jae},
    month={January},
    year={2024}
}

@misc{liu2023improvedllava,
      title={Improved Baselines with Visual Instruction Tuning}, 
      author={Liu, Haotian and Li, Chunyuan and Li, Yuheng and Lee, Yong Jae},
      publisher={arXiv:2310.03744},
      year={2023},
}

@misc{liu2023llava,
      title={Visual Instruction Tuning}, 
      author={Liu, Haotian and Li, Chunyuan and Wu, Qingyang and Lee, Yong Jae},
      publisher={NeurIPS},
      year={2023},
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">致谢</font></font></h2><a id="user-content-acknowledgement" class="anchor" aria-label="永久链接：致谢" href="#acknowledgement"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="https://github.com/lm-sys/FastChat"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Vicuna</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：我们构建的代码库，以及我们的基础模型 Vicuna-13B，它具有惊人的语言功能！</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">相关项目</font></font></h2><a id="user-content-related-projects" class="anchor" aria-label="永久链接：相关项目" href="#related-projects"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">使用 GPT-4 进行指令调整</font></font></a></li>
<li><a href="https://github.com/microsoft/LLaVA-Med"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">LLaVA-Med：一天内培训生物医学大型语言和视觉助理</font></font></a></li>
<li><a href="https://github.com/Luodian/Otter"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Otter：上下文内多模式指令调优</font></font></a></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">对于未来的项目想法，请查看：</font></font></p>
<ul dir="auto">
<li><a href="https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">SEEM：一次性分割各处的所有内容</font></font></a></li>
<li><a href="https://github.com/IDEA-Research/Grounded-Segment-Anything"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Grounded-Segment-Anything通过结合</font></font></a><font style="vertical-align: inherit;"></font><a href="https://github.com/IDEA-Research/GroundingDINO"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Grounding DINO</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><a href="https://github.com/facebookresearch/segment-anything"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">Segment-Anything</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">来检测、分割和生成任何东西</font><font style="vertical-align: inherit;">。</font></font></li>
</ul>
</article></div>
