# sagemaker-llm-hosting-workshop
Workshop for getting started with Hosting LLMs on SageMaker.

## Content

- [PyTorch Traditional Model Deployment](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/tree/master/traditional-model-deployment): In this section we focus on deploying a traditional pre-trained PyTorch Model to SageMaker Real-Time Inference.
- [Single LLM Deployment](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/tree/master/single-llm-deployment): We take a Llama 7B example with the LMI container and how to load test the deployed endpoint while enabling AutoScaling
- [Multi-LLM Deployment](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/tree/master/multi-llm-deployment): For use-cases where you have multiple LLMs or models we show how you can use Inference Components with SageMaker to efficiently allocate resources and host multiple models on a singular endpoint.