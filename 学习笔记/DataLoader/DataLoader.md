# DataLoader剖析

  + DataLoader本质是一个iterable（可迭代对象，类似于python内置类型List等），并利用多进程来加速batch data的处理；
  
  + DataLoader是一个高效简洁，直观的网络输入数据结构，便于使用和扩展；
  
## pytorch的数据加载到模型的操作顺序是：

   + 1、创建一个Dataset对象；
   
   + 2、创建一个DataLoader对象
   
   + 3、循环这个DataLoader对象，将graph、label加载到模型中训练。
   
            ‘’‘python
            
            dataset = MyDataset()
            
            dataloader = DataLoader(dataset)
            
            for epoch in range(num_epoches):
                ......
            
            ’‘’
    ```python
    #!/usr/bin/python3
    print("Hello, World!");
    ```
                
