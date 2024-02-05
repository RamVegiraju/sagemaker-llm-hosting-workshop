# Deploying Multiple LLMs on SageMaker Endpoint
In this example we will deploy multiple LLMs on a SageMaker Endpoint. With [SageMaker Inference Components](https://aws.amazon.com/blogs/aws/amazon-sagemaker-adds-new-inference-capabilities-to-help-reduce-foundation-model-deployment-costs-and-latency/), you can allocate hardware on a per model/container basis. In this example we will look at how you can host Llama and Flan on the same SageMaker Endpoint. For the Llama model we will utilize the LMI container in the single LLM Deployment and the TGI container for the FLAN Model Deployment.

## Additional Resources
- [TGI SageMaker Deployment](https://towardsdatascience.com/deploying-large-language-models-with-huggingface-tgi-981747c669e3)
- [Inference Components Amazon SageMaker Optimization](https://aws.amazon.com/blogs/machine-learning/reduce-model-deployment-costs-by-50-on-average-using-sagemakers-latest-features/)
- [Routing Optimizations](https://aws.amazon.com/blogs/machine-learning/minimize-real-time-inference-latency-by-using-amazon-sagemaker-routing-strategies/)