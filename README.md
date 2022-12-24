

# Quantum Computing via Amazon Braket


**Explore Amazon Bracket quantum computing to solve combinatorial optimization problems**

----

## Overview

* Explore the features and uses of the Amazon Braket console and components
* Discover benefits of quantum computing devices available on Amazon Braket, including gate quantum computers, annealer, and simulators
* Recognize which type of quantum device is the best fit for specific use cases and scaling
* Develop your own code from a basic set of use cases dealing with real-world optimization problems
* Understand the capabilities and limitations of current quantum computing technologies



----

## Instructions and Navigations
All of the code is organized into folders. For example, `Chapter03`.

Anyone running the code takes responsibility for any Amazon charges, and to review the code in detail to understand device costs and how many times a device is called from within a function to calculate total costs. Any accidental costs are not the responsibility of the Author.

-----


## Pricing Options

 Overview of Amazon Braket Pricing: [Amazon Pricing](https://aws.amazon.com/braket/pricing/)
 
 Tracking costs through code and setting limits: [Tracking Costs](https://docs.aws.amazon.com/braket/latest/developerguide/braket-pricing.html)
 
 AWS free tier for first time users : [Free Trial](https://aws.amazon.com/braket/pricing/?loc=ft#AWS_Free_Tier)

-----

## The Code

The code will look like the following:
```Python

from braket.aws import AwsDevice, AwsQuantumTask
from braket.circuits import Circuit
from braket.devices import LocalSimulator
# Set the number of shots 
n_shots = 10
# Use SV1 device
device = AwsDevice("arn:aws:braket:::device/quantum-simulator/amazon/sv1")
# Set the S3 bucket and folder name
my_bucket = "[bucket Name]" 
my_prefix = "[Folder Name]" 
s3_folder = (my_bucket, my_prefix)
# Define the quantum circuit
circ = Circuit().h(0).cnot(0, 1)
print(circ)
```



With the following software and hardware list you can run all code files present in the book (Chapter 1-13).

### Software and Hardware List

| Chapter  | Software required                   | OS required                        |
| -------- | ------------------------------------| -----------------------------------|
| 1-13        | Python and Jupyter Notebook                   | Windows |
| 1-13       | Amazon Braket SDK and Boto3             | Windows |
| 1-13        | D-Wave Ocean SDK             | Windows |


