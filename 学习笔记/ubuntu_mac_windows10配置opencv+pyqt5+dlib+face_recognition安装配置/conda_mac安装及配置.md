# 环境变量添加后出现prompt_status:5: command not found: wc错误导致所有终端指令无法使用？
                
   *解决方案：
                export PATH=/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin
                
   *问题：这样只能暂时解决,再次打开还是会出现同样的错误
                
   *彻底解决：
                
                mac如果是zsh终端，查看~/.zshrc文件，查看是否有 PATH= 后面没有包含 $PATH: 
                
                例如 export PATH=$PATH:$ANDROID_HOME/tools 

                或者 export PATH=$ANDROID_HOME/tools:$PATH

# conda创建虚拟环境

    
                
