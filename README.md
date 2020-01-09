# iFood ML Engineer Test

The goal of the exercises below is to evaluate the candidate knowledge and problem solving expertise regarding the main development focuses for the iFood ML Platform team: MLOps and Feature Store development.


## Sandbox: Feature Store building

Do you know what a feature store is? A feature store is a data provider serves features for machine learning models, both to its training and prediction phases.

As such, it must be able to provide data with consistency, reliability and flexibility. Data for for generating training datasets grows indefinitely, while data for realtime predictions must be available with low latency, while keeping the columns schema and values for the historical training data.

The goal for this exercise is to create a simple feature store.

### Requirements

* There's a kafka streaming for order events. Orders are made by clients, prepared by restaurants and delivered by drivers.
  * kafka #1: a49784be7f36511e9a6b60a341003dc2-1378330561.us-east-1.elb.amazonaws.com:9092
  * kafka #2: a4996369ef36511e9a6b60a341003dc2-1583999828.us-east-1.elb.amazonaws.com:9092
* Data needs to be consistent, we can’t lose anything.
* This processing pipeline needs to be scalable.

Feel free to use any solution to process and store this these data.

### Deliverable

* You're a ml engineer. Feel free to use any language and technology to reach your goal. Languages, frameworks, platforms are not a constraint, but your solution must be inside a docker image, docker compose, script or notebook ready to be run. Running this container/script or notebook should start reading the specified files and store it in a structured format.