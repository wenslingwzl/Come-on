# New journey

- 文档规范化管理过程记录

1.vim安装及其环境配置
遇到问题:
1) *startify: Can't read viminfo file. Read :help startify-faq-02*

   解决方案: 原始.vim文件备份 *mv .vim    .vim_backup*;
                       拷贝vim文件(网上或者别人转载的)到home路径下 *mv Downloads/vim   .vim*
                       (note:看vim支持python的版本, 这里是python3)
                       cd 到 *.vim/plugged/YouCompleteMe* 路径下,运行*./install.py --clang-completer*
                       问题解决!!!!

