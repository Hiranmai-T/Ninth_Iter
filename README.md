# Ninth_Iter

# Logs for 20 Epochs
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 17s 277us/step - loss: 0.5824 - acc: 0.8333 - val_loss: 0.1200 - val_acc: 0.9751
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 8s 128us/step - loss: 0.2651 - acc: 0.9205 - val_loss: 0.0696 - val_acc: 0.9834
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 8s 130us/step - loss: 0.2084 - acc: 0.9368 - val_loss: 0.0538 - val_acc: 0.9868
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 8s 129us/step - loss: 0.1801 - acc: 0.9431 - val_loss: 0.0438 - val_acc: 0.9884
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 8s 131us/step - loss: 0.1585 - acc: 0.9486 - val_loss: 0.0445 - val_acc: 0.9878
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 8s 130us/step - loss: 0.1433 - acc: 0.9518 - val_loss: 0.0385 - val_acc: 0.9894
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 8s 134us/step - loss: 0.1359 - acc: 0.9508 - val_loss: 0.0296 - val_acc: 0.9921
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 8s 131us/step - loss: 0.1286 - acc: 0.9518 - val_loss: 0.0285 - val_acc: 0.9918
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 8s 129us/step - loss: 0.1256 - acc: 0.9528 - val_loss: 0.0279 - val_acc: 0.9923
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 8s 129us/step - loss: 0.1182 - acc: 0.9536 - val_loss: 0.0265 - val_acc: 0.9935
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 8s 131us/step - loss: 0.1154 - acc: 0.9548 - val_loss: 0.0263 - val_acc: 0.9928
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 8s 128us/step - loss: 0.1101 - acc: 0.9550 - val_loss: 0.0252 - val_acc: 0.9929
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 8s 129us/step - loss: 0.1055 - acc: 0.9564 - val_loss: 0.0251 - val_acc: 0.9927
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 8s 129us/step - loss: 0.1050 - acc: 0.9557 - val_loss: 0.0211 - val_acc: 0.9941
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 8s 128us/step - loss: 0.1020 - acc: 0.9562 - val_loss: 0.0205 - val_acc: 0.9940
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 8s 129us/step - loss: 0.1006 - acc: 0.9573 - val_loss: 0.0217 - val_acc: 0.9943
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 8s 132us/step - loss: 0.0998 - acc: 0.9567 - val_loss: 0.0237 - val_acc: 0.9931
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 8s 133us/step - loss: 0.1003 - acc: 0.9563 - val_loss: 0.0223 - val_acc: 0.9936
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 8s 128us/step - loss: 0.0965 - acc: 0.9574 - val_loss: 0.0224 - val_acc: 0.9939
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 8s 129us/step - loss: 0.0983 - acc: 0.9555 - val_loss: 0.0212 - val_acc: 0.9944
<keras.callbacks.History at 0x7fe9e796c828>

# Model.evaluate
[0.021255379994329998, 0.9944]

# Approach
I figured in order to reduce the number of parameters, we have to either add maxPooling layer or 1x1 layer. When I added both 1x1 and maxPooling, the number of parameters got reduced but the accuracy went down. So, instead of adding both, I only added one 1x1 layer.The number of parameters decreased and I got 99.4 accuracy as required
