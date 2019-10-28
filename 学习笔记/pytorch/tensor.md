# Pytorch创建tensor的方法

  + 1、从numpy创建
  
             import torch
             
             import numpy as np
             
             a = np.array([2,3.3])
             
             a = torch.from_numpy(a)
             
             >>> tensor([2.0000,3.3000],dtype=torch.float64)
