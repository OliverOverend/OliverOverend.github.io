---
layout: post
title:  Microsoft Azure Machine Learning
comments: false
---
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