# CIFAR10-Authoencoder

## Autoencoder

*Encoder Structure*:

|Layer | Type | Maps | Size | Kernel | Stride | Pad. | Activ. |
| ---  | ---  | ---  | ---  | ---    | ---    | ---  | ---    |
|In | Input | 3 | 32$\times$32 | -  | - |- |  - |
|C1 | Conv. | 12 | 16$\times$16 | 4$\times$4  | 2 | 1 |  relu |
|C2 | Conv. | 24 | 8$\times$8 | 4$\times$4  | 2 | 1 | relu |
|C3 | Conv. | 48 | 4$\times$4 | 4$\times$4  | 2 | 1 | relu | 

*Decoder Structure*: 

|Layer | Type | Maps | Size | Kernel | Stride | Pad. | Activ. |
| ---  | ---  | ---  | ---  | ---    | ---    | ---  | ---    |
|In | Input       | 48 | 4$\times$4 | -  | - |- |  - |
|C1 | Trans.Conv. | 24 | 8$\times$8 | 4$\times$4  | 2 | 1 |  relu|
|C2 | Trans.Conv. | 12 | 16$\times$16 | 4$\times$4  | 2 | 1 |  relu|
|C3 | Trans.Conv. | 3 | 32$\times$32 | 4$\times$4 | 2 | 1 | tanh | 
    
    
    
