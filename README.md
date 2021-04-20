# CIFAR10-Authoencoder

## Autoencoder

*Encoder Structure*:

|Layer | Type | Maps | Size | Kernel | Stride | Pad. | Activ. |
| ---  | ---  | ---  | ---  | ---    | ---    | ---  | ---    |
|In | Input | 3 | 32x32 | -  | - |- |  - |
|C1 | Conv. | 12 | 16x16 | 4x4  | 2 | 1 |  relu |
|C2 | Conv. | 24 | 8x8 | 4x4  | 2 | 1 | relu |
|C3 | Conv. | 48 | 4x4 | 4x4  | 2 | 1 | relu | 

*Decoder Structure*: 

|Layer | Type | Maps | Size | Kernel | Stride | Pad. | Activ. |
| ---  | ---  | ---  | ---  | ---    | ---    | ---  | ---    |
|In | Input       | 48 | 4x4 | -  | - |- |  - |
|C1 | Trans.Conv. | 24 | 8x8 | 4x4  | 2 | 1 |  relu|
|C2 | Trans.Conv. | 12 | 16x16 | 4x4  | 2 | 1 |  relu|
|C3 | Trans.Conv. | 3 | 32x32 | 4x4 | 2 | 1 | tanh | 
    
    
    
