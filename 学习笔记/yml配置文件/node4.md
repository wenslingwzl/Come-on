# munch库的作用

  +  from munch import munchify

       +  作用：python convert dict to object like javascript
       
       + 参考网址：https://github.com/Infinidat/munch

# config.yml
    
 + 1.obj.toDict()
 
 + 2.obj.toJson()
 
 + 3.obj.toYaml()
 
 + 程序中应用---导入：xx = yaml.safe_load(file)
 
            Note:  需要注意的是随意在yaml里构建python对象是有一定危险的，尤其是接收到一个未知的yaml文档。yaml.safe_load可以限制这个能力，就使用些简单的对象吧


# json

  +  json.dumps(dict)  //字典转字符串
  
  + json.loads(string) //字符串转字典
  
  + json.dump(json_info,file)   //将json信息写进文件
  
  + file=open('x.json', 'r', encoding='utf-8')
     ----json.load(file)    //读取json信息
