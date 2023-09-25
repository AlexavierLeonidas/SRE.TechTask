# AWS CodePipeline Optimization Project

#Project Overview
This project employs AWS CodePipeline, a fully managed continuous delivery service, to automate the deployment workflows. The optimization of the pipeline is executed to perform only the tasks mentioned in the documentary, allowing for streamlined and efficient processes. The pipeline is broken into two main stages: Build and Deploy.

# Architecture
Stage 1: Build
This stage is broken into three phases:

Pre_Build: This phase involves logging into Amazon Elastic Container Registry (ECR) using Docker.

Build Stage: In this phase, the Docker image is constructed.

Post_Build: The post-build phase is responsible for pushing the created Docker image into ECR, updating the Amazon Elastic Container Service (ECS), and generating the definition.json.

Stage 2: Deploy
This stage takes care of deploying the built Docker image using Amazon ECS.

# Deployment Result
To view the deployment result, please visit 52.91.61.156:80.

# Rationale
Selection of AWS CodePipeline
AWS CodePipeline was chosen for this project due to its seamless integration with other AWS services, enabling a smooth and efficient deployment pipeline. Its fully managed service offers capabilities to model, visualize, and automate the steps required to release software, thereby providing reliable and faster delivery.

Optimization Strategy
The optimization of the pipeline was undertaken to align strictly with the tasks specified in the documentary. This alignment ensures that there are no redundant or unnecessary steps in the pipeline, promoting efficiency and reducing the likelihood of errors.

The pipeline’s structure, consisting of well-defined stages and phases, allows for clear segmentation of tasks, making the workflow easier to understand, manage, and troubleshoot.

# Why AWS CodePipeline and this Optimization?
Efficiency: By focusing solely on the tasks mentioned in the documentary, unnecessary overhead is eliminated, allowing for quicker deployments.
Reliability: AWS CodePipeline offers a reliable platform to automate the deployment process, ensuring consistent results with every execution.
Integration: The use of AWS services such as ECR and ECS provides seamless integration and a cohesive environment for deployment tasks.
Scalability: The AWS platform offers scalability, allowing the pipeline to adapt to increasing loads when needed.
Conclusion
This optimized AWS CodePipeline serves as an effective solution for streamlined and reliable software deployments, by leveraging AWS services and adhering strictly to the tasks outlined in the documentary. The deployed results can be viewed and verified by accessing the provided public IP address.

# Access the Deployment
The deployment can be viewed by visiting the following link: http://52.91.61.156:80.

# In Addition, I have attached the task_definition.json file.