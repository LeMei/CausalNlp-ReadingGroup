## Background

Counterfactual Reasoning（反事实推理）与Causal Inference（因果推断）和Causal Intervention（因果干预）之间有密切的关系。这三者都是因果推理体系的重要组成部分，各自作用不同但相互联系紧密。

[Causal inference in statistics: A primer](https://books.google.dk/books?hl=da&lr=&id=I0V2CwAAQBAJ&oi=fnd&pg=PR9&dq=Causal+inference+in+statistics:+A+primer.+John+Wiley+%26+Sons.&ots=9BnXAuZNkj&sig=LwMZSeEruDuLis6rnquWb2E6mNM&redir_esc=y#v=onepage&q=Causal%20inference%20in%20statistics%3A%20A%20primer.%20John%20Wiley%20%26%20Sons.&f=false)

[Causal Inference in the Record of the SAT Scores](https://spa-drp.github.io/writeups/aut2021/slides/hadi.pdf)

[Direct and indirect effects](https://arxiv.org/pdf/1301.2300)

**1. Counterfactual Reasoning（反事实推理）**

反事实推理的核心是回答“如果当时不同，会发生什么？”这种假设性问题，即探索实际事件未发生的情境下可能的结果。反事实推理在因果推断和干预中扮演了重要角色，尤其在理解和预测不同情境下的潜在结果时。

典型问题：反事实推理关注的是一个变量的值在不同情境下可能会导致的结果。比如，“如果我没有接受治疗，我的健康状况会怎样？”即使治疗已经发生，反事实推理尝试估计在未接受治疗的假设下的结果。
实现方式：反事实推理常基于已构建的因果模型，通过改变其中一个或多个条件来评估假设情境。例如，裴金斯提出的三层因果模型（关联、干预和反事实）中的第三层就专门描述了反事实推理。

**2. Causal Inference（因果推断）与 Counterfactual Reasoning 的关系**

目的和方法：因果推断的主要目的是识别和估计真实世界中的因果关系，而反事实推理是其中的一部分，专门用于推测在不同情况下的因果结果。
潜在结果框架：反事实推理通常依赖于潜在结果框架（Potential Outcomes Framework），其中会考虑在处理和未处理情境下的结果。因果推断模型可帮助计算这些潜在结果，从而完成反事实推理。
因果推断验证反事实推理：通过因果推断可以评估反事实推理的准确性，例如，通过实验证明干预是否真正有效，来验证反事实的合理性。

**3. Causal Intervention（因果干预）与 Counterfactual Reasoning 的关系**

干预作为反事实的基础：因果干预中直接涉及反事实推理，因为干预前后结果的差异可以被视为一种反事实。


反事实验证干预效果：反事实推理允许我们在干预操作上进行假设性推断。例如，我们可以模拟出一个反事实情境，评估干预对不同条件下的效果，这在政策和医学干预中尤为关键。
三者的关系总结
因果推断是基础：首先，通过因果推断理解变量之间的因果关系。
干预是操作手段：在此因果关系模型上，干预能够提供一种实际操作，通过更改变量的状态来测试模型。
反事实推理是预测和评估方法：反事实推理利用因果关系和干预的结果进行假设性推断，帮助预测未发生的情境下的可能后果。


Zhijing jin talk, take away

-better casual reasoning for LLMs
-a causal framework for different NLP task
-interpretion


Hallcatio
Structure reasoning + API + LLM

fact-checking

correlation =? causality

we don't want interpret the past but to act towards the future
what causes what

causal graph types: 
dataset: corr2cause, it is about exploration of relation between correlation and causality

corr2cause

prompt-> correlational statements--> LLM --> judgement of causality


future work:

1. causal discovery by LLM from data
2. causal metric for specific domain


commonsense causality--- cutting-edge reasoning 


*** causal question ***  depending on the specific task, help us to make decision on normal question in daily life
----formalize QA as causal questions and combine many factors by causal graph for decision making.

*** Formulate Nlp task with causal framework***

personalization (with user information/background or not), i.e., implicit and explicit

cultural role (adaptivity, discrimination) in causal reasoning of LLMs, whether llm provide a correct or wrong fact with the user culture background (indeed influenced by culture for most LLMs)

LLMs tailer responses for desesired IP and undesired IP

the causlality between culture background and response for LLMs. 
Is the users' ip address cause different responses? (why it happens), interpretion
response bias cause by culture background

causal discovery of category (people group) known by LLMs
counter-fact on category 


1. improve causal reasoning 






















