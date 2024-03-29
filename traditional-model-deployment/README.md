# Deploying Traditional Models on Amazon SageMaker

In this section we'll take a look at how we can deploy traditional pre-trained models on Amazon SageMaker Real-Time Inference. We will use the Boto3 Python SDk with a pre-trained PyTorch model for deployment. Note that there are different ways that you can deploy pre-trained models including the [SageMaker Model Builder Class](https://github.com/aws-samples/sagemaker-hosting/tree/main/SageMaker-Model-Builder) and SageMaker Python SDK which might be simpler in specific use-cases.

## Content

- [single-model-deployment](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/tree/master/traditional-model-deployment/single-model-deployment): Focusing on deployment of a single model endpoint.
    - [pretrained-torch-example.ipynb](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/blob/master/traditional-model-deployment/single-model-deployment/pretrained-torch-example.ipynb): Training a sample PyTorch model locally and deploying the model artifacts to SageMaker Inference using the Boto3 SDK.
    - [bert-deployment.ipynb](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/blob/master/traditional-model-deployment/single-model-deployment/bert-deployment.ipynb): Taking a HuggingFace BERT Model and generated code from the HuggingFace Hub to directly deploy to a single model endpoint with the SageMaker Python SDK.
- [multi-model-deployment](https://github.com/RamVegiraju/sagemaker-llm-hosting-workshop/tree/master/traditional-model-deployment/multi-model-endpoints): An example utilizing the built-in Multi-Model Endpoint (MME Solution) to host hundreds of sample SKLearn models on a singular endpoint. You can replace the SKLearn code with whatever PyTorch model artifact and model.py adjustments as needed to load and work with the model.

## Additional Resources

- [SageMaker Multi-Model Endpoints](https://docs.aws.amazon.com/sagemaker/latest/dg/multi-model-endpoints.html)
- [Pre-Trained Model Deployment](https://sagemaker-examples.readthedocs.io/en/latest/sagemaker-script-mode/pytorch_bert/deploy_bert_outputs.html)