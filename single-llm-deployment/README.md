# LLM Deployment
In this example we focus on deploying a singular LLM on SageMaker Real-Time Inference. For this we will utilize the Large Model Inference Container (LMI) managed by AWS. With the LMI container we can enable optimizations such as Batching, Quantization, and more. The LMI containers comes enabled with a variety of different model partitioning tools such as DeepSpeed, Accelerate and more. To understand the latest optimized LMI container we will use refer to this [launch](https://aws.amazon.com/blogs/machine-learning/boost-inference-performance-for-llms-with-new-amazon-sagemaker-containers/).

## Load-Testing & AutoScaling
In this example we also enable load testing via [Locust](https://locust.io/). Here you can adjust the distributed.sh to adjust your concurrency for tests. AutoScaling is also enabled to scale up based off of the TPM that you have set.

## Additional Resources
- [Load Testing SageMaker Endpoints with Locust](https://aws.amazon.com/blogs/machine-learning/best-practices-for-load-testing-amazon-sagemaker-real-time-inference-endpoints/)
- [AutoScaling SageMaker Endpoints](https://towardsdatascience.com/autoscaling-sagemaker-real-time-endpoints-b1b6e6731c59)
- [LMI Container Introduction](https://towardsdatascience.com/deploying-llms-on-amazon-sagemaker-with-djl-serving-8220e3cfad0c)
- [LMI TensorRT Blog](https://aws.amazon.com/blogs/machine-learning/boost-inference-performance-for-llms-with-new-amazon-sagemaker-containers/)