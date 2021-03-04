# iFood ML Engineer Test

The goal of the exercises below is to evaluate the candidate knowledge and problem solving expertise regarding the main development focuses for the iFood ML Platform team: MLOps and Feature Store development.


## Feature Store building

A feature store is a data provider that serves features for machine learning models, both to its training and prediction phases.

As such, it must be able to provide data with consistency, reliability and flexibility. Data for for generating training datasets grows indefinitely, while data for realtime predictions must be available with low latency, while keeping the columns schema and values for the historical training data.

The goal for this exercise is to create a simple feature store.

### Setup

* There are four source files, available at:
  - https://ifood-data-architect-test-source.s3-sa-east-1.amazonaws.com/order.json.gz
  - https://ifood-data-architect-test-source.s3-sa-east-1.amazonaws.com/consumer.csv.gz
  - https://ifood-data-architect-test-source.s3-sa-east-1.amazonaws.com/restaurant.csv.gz
  - https://ifood-data-architect-test-source.s3-sa-east-1.amazonaws.com/status.json.gz
* Please emulate a streaming source based on those files
* Data needs to be consistent, we can’t lose anything.
* This processing pipeline needs to be scalable.

Feel free to use any solution to process and store this data.

### Deliverable

* You're a ML Engineer. Feel free to use any language and technology to reach your goal. Languages, frameworks, platforms are not a constraint, but your solution must be inside a docker image, docker compose, script or notebook ready to be run. Running this container/script or notebook should start reading the specified files and store the results in a structured format.

## ML model serving

Part of the ML Engineer job is to ensure the models developed by the Data Scientists are correctly deployed to the production environment, and are accessible via a REST microservice.

### Deliverables

There are two goals for this exercise. The first one is to create an automated ML model training process.

The second one is to create a Rest API documented with Swagger that serves a ML model predictions.

This process/pipeline should be generic enough to implement any models, with any data.

Languages, frameworks, platforms are not a constraint, but your solution must be inside a docker image, docker compose, script or notebook ready to be run. Training a model or serving the Rest API/Swagger structure should be as simple as running a script or something similar. You should also provide a README file on how to execute the training job, and how to request the API or Swagger. There are a lot of tools that solve most of this problem; while you are free to use them, please try to balance the time you will save by using them with being able to show your programming skills by not using them as much.

## AWS infrastructure

The last skill a ML Engineer must have is cloud proficiency. For iFood, AWS is our cloud of choice.

For this exercise, we would like for you to propose an AWS architecture to serve a solution for one of the two previous exercises. A single page describing the resources needed is sufficient, although you are free to provide code if you like it. Please have in mind that this structure must be reliable, scalable and as cheap as possible without compromising the other two requisites.

## BONUS!!

These exercises are all optional! They are not required to evaluate how you'll perform in this job, and they require no skills listed in the job description whatsoever! They are fun and difficult, though 😈

Let's get to it!

### Level 1 and 2

Can you figure out the passwords for the binaries `bonus/level01` and `bonus/level02`?

### Level 3

Can you get a shell from the binary `bonus/level03`?

```
 Ex.
 $ ./bonus/level03
 [+] calling some crazy function, can you get a shell?
 password: something_that_executes_/bin/sh
 $ echo "Habemus shell!"
```
