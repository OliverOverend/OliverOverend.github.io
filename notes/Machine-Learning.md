---
layout: post
title: Machine learning
comments: false
---
- [Explaining generative language models to (almost) anyone](https://stackoverflow.blog/2024/06/27/explaining-generative-language-models-to-almost-anyone/)
- [Partial Dependence Plots](https://www.blog.trainindata.com/partial-dependence-plots-with-python/#:~:text=Step%2Dby%2DStep%20Guide%20to%20Creating%20Partial%20Dependence%20Plots&text=Select%20the%20feature%20of%20interest,variable%20using%20the%20trained%20model.)
- [Partial Dependence Plots](https://christophm.github.io/interpretable-ml-book/pdp.html#pdp)
- [LIME plots](https://christophm.github.io/interpretable-ml-book/lime.html)
- [ICE plots](https://christophm.github.io/interpretable-ml-book/ice.html)
- [Interpretable Machine Learning](https://christophm.github.io/interpretable-ml-book/)
- [A Visual Exploration of Gaussian Processes](https://distill.pub/2019/visual-exploration-gaussian-processes)
- [Efficient Machine Learning Inference](https://www.oreilly.com/content/efficient-machine-learning-inference/)
- [Responsible AI: The Role of Data and Model Cards](https://datatonic.com/insights/responsible-ai-data-model-cards/)
- [Rules of Machine Learning](https://developers.google.com/machine-learning/guides/rules-of-ml/)
- [Minimizing real-time prediction serving latency in machine learning](https://cloud.google.com/architecture/minimizing-predictive-serving-latency-in-machine-learning)
- [Introduction to the Azure ML-Ops Project Accelerator](https://microsoft.github.io/azureml-ops-accelerator/)
- [ML Ops Github List](https://github.com/stars/OliverOverend/lists/ml-ops/)
- [Phase Zero](https://ml-ops.org/content/phase-zero)
- [MLOps Stack Canvas](https://ml-ops.org/content/mlops-stack-canvas)


- [The 2019 Accelerate State of DevOps: Elite performance, productivity, and scaling](https://cloud.google.com/blog/products/devops-sre/the-2019-accelerate-state-of-devops-elite-performance-productivity-and-scaling)
- [Introduction to Azure Storage](https://learn.microsoft.com/en-us/azure/storage/common/storage-introduction)
- [Azure GitHub List](https://github.com/stars/OliverOverend/lists/azure/)

- [Machine Learning operations](https://learn.microsoft.com/en-gb/azure/cloud-adoption-framework/ready/azure-best-practices/ai-machine-learning-mlops)
- [Network isolation with Azure Machine Learning registries](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-registry-network-isolation)
- [Share models, components, and environments across workspaces with registries](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-share-models-pipelines-across-workspaces-with-registries)
- [Set up MLOps with Azure DevOps](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-setup-mlops-azureml)
- [Network isolation with managed online endpoints](https://learn.microsoft.com/en-us/azure/machine-learning/concept-secure-online-endpoint)
- [Manage and increase quotas and limits for resources with Azure Machine Learning](https://learn.microsoft.com/en-us/azure/machine-learning/how-to-manage-quotas)
- [Autoscaling](https://learn.microsoft.com/en-us/azure/architecture/best-practices/auto-scaling)

Limitations:
- Inability to deploy multiple registered models to a deployment
- Inability to get the image build status when building a custom environment in a CICD pipeline
- Inability to see the managed endpoint quota limits in a UI
- Inability to downgrade SKU without causing downtime
- Scaling out instances is rather slow, therefore auto-scaling rules need to be preemptive. Downtime is to expected in certain outage scenarios or in unexpected surges of demand.
- When the outbound access is secured, can we access a storage account?
