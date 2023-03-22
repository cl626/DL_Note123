1. pytorch有哪些常用的优化器，调用格式是怎样的？

![image-20230322160621657](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322160621657.png)

![image-20230322160633055](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322160633055.png)

* ==Other parameter==👉weight_decay，

```python
optimizer=torch.optim.Adam(net.parameters(),lr=learning_rate,weight_decay=weight_decay)
```

2. python中assert函数的作用？

![image-20230322162154431](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322162154431.png)

3. torch数组的拼接可以直接用“+”吗？

![image-20230322163204532](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322163204532.png)

4. torch数组可以直接用索引来分割吗？

![image-20230322164747149](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322164747149.png)

但==切片索引必须是整数或 None 或具有 __index__ 方法==

而多元数组维数索引较麻烦，

5. torch.slice的作用？

![image-20230322165043449](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322165043449.png)

6. python 变量前加*的作用？

![image-20230322165648222](../../Users/c1826/AppData/Roaming/Typora/typora-user-images/image-20230322165648222.png)

7. slice的作用？——``` slice(start, stop, step)```,作为索引
