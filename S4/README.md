## Model Architecture ## 

## Note the average pooling is applied in forward function ##

----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1          [-1, 128, 28, 28]           3,328
              ReLU-2          [-1, 128, 28, 28]               0
       BatchNorm2d-3          [-1, 128, 28, 28]             256
           Dropout-4          [-1, 128, 28, 28]               0
            Conv2d-5            [-1, 8, 30, 30]           1,032
            Conv2d-6           [-1, 16, 30, 30]           1,168
              ReLU-7           [-1, 16, 30, 30]               0
       BatchNorm2d-8           [-1, 16, 30, 30]              32
           Dropout-9           [-1, 16, 30, 30]               0
        MaxPool2d-10           [-1, 16, 15, 15]               0
           Conv2d-11           [-1, 16, 15, 15]           6,416
             ReLU-12           [-1, 16, 15, 15]               0
      BatchNorm2d-13           [-1, 16, 15, 15]              32
          Dropout-14           [-1, 16, 15, 15]               0
        MaxPool2d-15             [-1, 16, 7, 7]               0
           Conv2d-16             [-1, 16, 7, 7]           2,320
             ReLU-17             [-1, 16, 7, 7]               0
      BatchNorm2d-18             [-1, 16, 7, 7]              32
          Dropout-19             [-1, 16, 7, 7]               0
           Conv2d-20              [-1, 8, 9, 9]             136
           Linear-21                   [-1, 10]           5,130
================================================================
Total params: 19,882
Trainable params: 19,882
Non-trainable params: 0

----------------------------------------------------------------
Input size (MB): 0.00
Forward/backward pass size (MB): 3.73
Params size (MB): 0.08
Estimated Total Size (MB): 3.81
----------------------------------------------------------------
<ipython-input-28-f32fef0cdb4a>:52: UserWarning: Implicit dimension choice for log_softmax has been deprecated. Change the call to include dim=X as an argument.
  return  F.log_softmax(output)   # return x for visualization
  
  
  ######## Logs #######################
  
  
  
  
  epoch value is ,  1
  0%|          | 0/469 [00:00<?, ?it/s]<ipython-input-28-f32fef0cdb4a>:52: UserWarning: Implicit dimension choice for log_softmax has been deprecated. Change the call to include dim=X as an argument.
  return  F.log_softmax(output)   # return x for visualization
loss=0.1726485937833786 batch_id=468: 100%|██████████| 469/469 [00:20<00:00, 23.06it/s]

Test set: Average loss: 0.0986, Accuracy: 9691/10000 (97%)

epoch value is ,  2
loss=0.02403418719768524 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.96it/s]

Test set: Average loss: 0.0323, Accuracy: 9902/10000 (99%)

epoch value is ,  3
loss=0.027550719678401947 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.89it/s]

Test set: Average loss: 0.0283, Accuracy: 9906/10000 (99%)

epoch value is ,  4
loss=0.0842796340584755 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 28.03it/s]

Test set: Average loss: 0.0300, Accuracy: 9896/10000 (99%)

epoch value is ,  5
loss=0.0314621664583683 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 27.06it/s]

Test set: Average loss: 0.0230, Accuracy: 9921/10000 (99%)

epoch value is ,  6
loss=0.02799431048333645 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 28.02it/s]

Test set: Average loss: 0.0279, Accuracy: 9908/10000 (99%)

epoch value is ,  7
loss=0.0137522853910923 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 26.93it/s]

Test set: Average loss: 0.0231, Accuracy: 9929/10000 (99%)

epoch value is ,  8
loss=0.01810109056532383 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 26.68it/s]

Test set: Average loss: 0.0233, Accuracy: 9930/10000 (99%)

epoch value is ,  9
loss=0.09114695340394974 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 26.34it/s]

Test set: Average loss: 0.0220, Accuracy: 9927/10000 (99%)

epoch value is ,  10
loss=0.036803558468818665 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.68it/s]

Test set: Average loss: 0.0207, Accuracy: 9937/10000 (99%)

epoch value is ,  11
loss=0.03330874443054199 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 27.15it/s]

Test set: Average loss: 0.0182, Accuracy: 9944/10000 (99%)

epoch value is ,  12
loss=0.026055367663502693 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 26.44it/s]

Test set: Average loss: 0.0239, Accuracy: 9928/10000 (99%)

epoch value is ,  13
loss=0.004545198287814856 batch_id=468: 100%|██████████| 469/469 [00:17<00:00, 27.58it/s]

Test set: Average loss: 0.0180, Accuracy: 9938/10000 (99%)

epoch value is ,  14
loss=0.004932833835482597 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.66it/s]

Test set: Average loss: 0.0225, Accuracy: 9932/10000 (99%)

epoch value is ,  15
loss=0.0004928396665491164 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.76it/s]

Test set: Average loss: 0.0182, Accuracy: 9944/10000 (99%)

epoch value is ,  16
loss=0.0180299561470747 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.71it/s]

Test set: Average loss: 0.0176, Accuracy: 9948/10000 (99%)

epoch value is ,  17
loss=0.0023433775641024113 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.64it/s]

Test set: Average loss: 0.0194, Accuracy: 9947/10000 (99%)

epoch value is ,  18
loss=0.003397254506126046 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.86it/s]

Test set: Average loss: 0.0175, Accuracy: 9941/10000 (99%)

epoch value is ,  19
loss=0.0004057574551552534 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 27.80it/s]

Test set: Average loss: 0.0185, Accuracy: 9946/10000 (99%)

epoch value is ,  20
loss=0.00013964359823148698 batch_id=468: 100%|██████████| 469/469 [00:16<00:00, 28.04it/s]

Test set: Average loss: 0.0208, Accuracy: 9934/10000 (99%)

  
  
  
