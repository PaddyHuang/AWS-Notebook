# AWS Storage Services

AWS Storage Services ranges from *object*, *block*, to *file* storage, with some supporting services, mainly as below.

| Services Type |Keywords|AWS Services|
|:-------------:|:-------|:----------:|
|Object Storage |1. Key-value, 2. Unstructured|Amazon S3|
|Block Storage  |1. Fix-size block|Amazon EBS|
|File Storage   |1. File system, 2. Structured|Amazon EFS Amazon FSx|

Comparison:

|            Features            |                              S3                              |                    EBS                     |          EFS           |
| :----------------------------: | :----------------------------------------------------------: | :----------------------------------------: | :--------------------: |
|          Storage Type          |                           Objects                            |                   Block                    |          File          |
|          Storage Size          |                          Unlimited                           |                  Max 16TB                  |       Unlimited        |
| Size Limitation for Each Files |                         0bytes ~ 5TB                         |                 Unlimited                  |        Max 52TB        |
|              IOPS              | Multipart Upload Sopported. If only use single object upload, restrained to 5GB/s | SSD or HDD Supported meeting variaous IOPS |     3GB Defaultly      |
|             Access             |                         via Internet                         |                 Single EC2                 | Up to thousands of EC2 |
|          Availability          |                            99.99%                            |                   99.99%                   |          High          |
|             Speed              |                           Slowest                            |                  Fastest                   |         Medium         |
|            Pricing             |                            Lowest                            |                   Medium                   |        Highest         |

