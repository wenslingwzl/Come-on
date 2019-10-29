# Pytorch创建tensor的方法

  + 1、从numpy创建
  
             import torch
             
             import numpy as np
             
             a = np.array([2,3.3])
             
             a = torch.from_numpy(a)
             
             >>> tensor([2.0000,3.3000],dtype=torch.float64)
  + 2、随机初始化
  
              # 采样自0~1均匀分布
              
              a = torch.rand(3, 3)
              
              >>> tensor 3*3的矩阵，取值0-1
              
              # 形如*_like接受一个Tensor,将这个Tensor的shape读取出来之后在送入*所表示的函数

              # 下面的rand_like(a)即将a的shape=3,3读出来传给torch.rand()函数
               
              b = torch.rand_like(a)  # 相当于执行了torch.rand(3,3)

              # 在区间[1,10)上随机采样,生成shape=2,2的LongTensor

              c = torch.randint(1, 10, [2, 2])

              # 采样自N(0,1)

              d = torch.randn(3, 3)
              
# 运行代码时出现 No module named 'torch_scatter'？

 +  pip install --verbose --no-cache-dir torch-scatter
    
 + pip install --verbose --no-cache-dir torch-sparse
    
 + pip install --verbose --no-cache-dir torch-cluster
    
  +  pip install torch-geometric
    
  + 具体参考：https://github.com/rusty1s/pytorch_geometric   中Installation部分的介绍。
