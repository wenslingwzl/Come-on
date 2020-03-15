# 环境变量添加后出现prompt_status:5: command not found: wc错误导致所有终端指令无法使用？
                
   * 解决方案：
                export PATH=/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin
                
   * 问题：这样只能暂时解决,再次打开还是会出现同样的错误
                
   * 彻底解决：
                
                mac如果是zsh终端，查看~/.zshrc文件，查看是否有 PATH= 后面没有包含 $PATH: 
                
                例如 export PATH=$PATH:$ANDROID_HOME/tools 

                或者 export PATH=$ANDROID_HOME/tools:$PATH

# conda创建虚拟环境

   * conda create -n your_env_name python=X.X（2.7、3.7等)
   
# 删除虚拟环境

  * conda remove --name env_name --all

# 虚拟环境之间的切换/推出虚拟环境

  * source activate env_name
  
  * source deactivate env_name
  
# MAC中Python如何通过pip将packages安装到Conda环境中?
   
  * source到创建的虚拟环境中conda install pip ，它会将pip安装到虚拟环境目录中，之后pip install package_name即可。
  
   

    
                
