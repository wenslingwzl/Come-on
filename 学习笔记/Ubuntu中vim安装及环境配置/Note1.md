# vim安装及其环境配置

遇到问题:

* *startify: Can't read viminfo file. Read :help startify-faq-02?*

   解决方案
   
             原始.vim文件备份  mv .vim    .vim_backup
                       
             拷贝vim文件(网上或者别人转载的这里scp -r xxx@123.123.0.123:~/.vim Downloads/vim)到home路径下  mv Downloads/vim   .vim
                       
             (note:看vim支持python的版本, 这里是python3)
                       
             cd 到 *.vim/plugged/YouCompleteMe 路径下,运行*./install.py --clang-completer
                       
             问题解决!!!!
             
* *vim出现无法写入，已设定选项‘buftype’*

   解决方案
   
            ！！没有弄明白：网上说修改buftype的方法：
            
            vim切换至ex模式，输入 :setlocal buftype= （为空时）才能写入———尝试无效果
            
            关闭窗口重新打开----能够写入？？
