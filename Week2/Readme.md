
# **Week2 Assignment**



**Logs of 20 Epochs:**

```
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 8s 127us/step - loss: 0.5158 - acc: 0.8543 - val_loss: 0.0859 - val_acc: 0.9853
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 6s 96us/step - loss: 0.2501 - acc: 0.9256 - val_loss: 0.0618 - val_acc: 0.9865
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1966 - acc: 0.9419 - val_loss: 0.0411 - val_acc: 0.9901
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 6s 94us/step - loss: 0.1688 - acc: 0.9456 - val_loss: 0.0393 - val_acc: 0.9901
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1526 - acc: 0.9492 - val_loss: 0.0342 - val_acc: 0.9900
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 6s 94us/step - loss: 0.1412 - acc: 0.9504 - val_loss: 0.0269 - val_acc: 0.9924
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1312 - acc: 0.9523 - val_loss: 0.0249 - val_acc: 0.9926
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1252 - acc: 0.9524 - val_loss: 0.0231 - val_acc: 0.9928
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1192 - acc: 0.9537 - val_loss: 0.0265 - val_acc: 0.9922
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1156 - acc: 0.9544 - val_loss: 0.0220 - val_acc: 0.9935
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1135 - acc: 0.9548 - val_loss: 0.0236 - val_acc: 0.9922
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 6s 95us/step - loss: 0.1097 - acc: 0.9546 - val_loss: 0.0222 - val_acc: 0.9936
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 6s 96us/step - loss: 0.1070 - acc: 0.9556 - val_loss: 0.0210 - val_acc: 0.9934
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 6s 98us/step - loss: 0.1038 - acc: 0.9565 - val_loss: 0.0210 - val_acc: 0.9938
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 6s 97us/step - loss: 0.1016 - acc: 0.9566 - val_loss: 0.0202 - val_acc: 0.9948
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 6s 94us/step - loss: 0.1005 - acc: 0.9553 - val_loss: 0.0206 - val_acc: 0.9937
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 6s 95us/step - loss: 0.0990 - acc: 0.9569 - val_loss: 0.0208 - val_acc: 0.9936
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 6s 95us/step - loss: 0.0973 - acc: 0.9570 - val_loss: 0.0222 - val_acc: 0.9925
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 6s 95us/step - loss: 0.0986 - acc: 0.9553 - val_loss: 0.0209 - val_acc: 0.9938
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 6s 94us/step - loss: 0.0938 - acc: 0.9583 - val_loss: 0.0202 - val_acc: 0.9941
<keras.callbacks.History at 0x7f6ec1ce53c8>
```





**Result of  model.evaluate (on test data):**

 [0.020171252903481946, 0.9941] 



**Strategy:**

Started with 8 channels instead of 16.

```
Model: "sequential_4"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_13 (Conv2D)           (None, 26, 26, 8)         72        
_________________________________________________________________
batch_normalization_10 (Batc (None, 26, 26, 8)         32        
_________________________________________________________________
dropout_10 (Dropout)         (None, 26, 26, 8)         0         
_________________________________________________________________
conv2d_14 (Conv2D)           (None, 24, 24, 10)        720       
_________________________________________________________________
batch_normalization_11 (Batc (None, 24, 24, 10)        40        
_________________________________________________________________
dropout_11 (Dropout)         (None, 24, 24, 10)        0         
_________________________________________________________________
conv2d_15 (Conv2D)           (None, 24, 24, 10)        100       
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 12, 12, 10)        0         
_________________________________________________________________
conv2d_16 (Conv2D)           (None, 10, 10, 16)        1440      
_________________________________________________________________
batch_normalization_12 (Batc (None, 10, 10, 16)        64        
_________________________________________________________________
dropout_12 (Dropout)         (None, 10, 10, 16)        0         
_________________________________________________________________
conv2d_17 (Conv2D)           (None, 8, 8, 16)          2304      
_________________________________________________________________
batch_normalization_13 (Batc (None, 8, 8, 16)          64        
_________________________________________________________________
dropout_13 (Dropout)         (None, 8, 8, 16)          0         
_________________________________________________________________
conv2d_18 (Conv2D)           (None, 6, 6, 16)          2304      
_________________________________________________________________
batch_normalization_14 (Batc (None, 6, 6, 16)          64        
_________________________________________________________________
dropout_14 (Dropout)         (None, 6, 6, 16)          0         
_________________________________________________________________
conv2d_19 (Conv2D)           (None, 4, 4, 16)          2304      
_________________________________________________________________
batch_normalization_15 (Batc (None, 4, 4, 16)          64        
_________________________________________________________________
dropout_15 (Dropout)         (None, 4, 4, 16)          0         
_________________________________________________________________
conv2d_20 (Conv2D)           (None, 1, 1, 10)          2560      
_________________________________________________________________
batch_normalization_16 (Batc (None, 1, 1, 10)          40        
_________________________________________________________________
dropout_16 (Dropout)         (None, 1, 1, 10)          0         
_________________________________________________________________
flatten_2 (Flatten)          (None, 10)                0         
_________________________________________________________________
activation_2 (Activation)    (None, 10)                0         
=================================================================
Total params: 12,172
Trainable params: 11,988
Non-trainable params: 184
_________________________________________________________________
/usr/local/lib/python3.6/dist-packages/ipykernel_launcher.py:36: UserWarning: Update your `Conv2D` call to the Keras 2 API: `Conv2D(10, (4, 4), use_bias=False)`
```

