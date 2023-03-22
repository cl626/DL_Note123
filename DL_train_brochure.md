##### python基础

1. python中assert函数的作用？

![image-20230322162154431](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322162154431.png)

2. slice的作用？——``` slice(start, stop, step)```,作为列表的索引

3. python 变量前加*的作用？

![image-20230322165648222](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322165648222.png)

##### torch 数组基本操作

1. torch数组的拼接可以直接用“+”吗？

![image-20230322163204532](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322163204532.png)

2. torch数组可以直接用索引来分割吗？

![image-20230322164747149](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322164747149.png)

但==切片索引必须是整数或 None 或具有 __index__ 方法==

而多元数组维数索引较麻烦，

3. torch.slice的作用？

![image-20230322165043449](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322165043449.png)

##### torch.utils.data(数据—pandas→torch)

1. 如何替换```train_iter=d2l.load_array([train_features,train_labels],batch_size)```

```python
import torch.utils.data as data

train_dataset = data.TensorDataset(train_features, train_labels)
train_dataloader = data.DataLoader(train_dataset, batch_size=batch_size)
```

![image-20230322195404432](https://raw.githubusercontent.com/cl626/Image/master/Picgo/image-20230322195404432.png)

![image-20230322195421625](https://raw.githubusercontent.com/cl626/Image/master/Picgo/image-20230322195421625.png)

##### torch.nn

###### neural_network

![image-20230322200529933](https://raw.githubusercontent.com/cl626/Image/master/Picgo/image-20230322200529933.png)

###### loss_function ![image-20230322201256873](https://raw.githubusercontent.com/cl626/Image/master/Picgo/image-20230322201256873.png)

###### example

![image-20230322201346571](https://raw.githubusercontent.com/cl626/Image/master/Picgo/image-20230322201346571.png)

##### torch.optim(优化器)

1. pytorch有哪些常用的优化器，调用格式是怎样的？

![image-20230322160621657](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322160621657.png)

![image-20230322160633055](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322160633055.png)

* ==Other parameter==👉weight_decay，

```python
optimizer=torch.optim.Adam(net.parameters(),lr=learning_rate,weight_decay=weight_decay)
```
