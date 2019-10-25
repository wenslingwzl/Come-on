# munch库的作用

  +  from munch import munchify

       +  作用：python convert dict to object like javascript
       
       + 参考网址：https://github.com/Infinidat/munch

# config.yml
    
 + 1.obj.toDict()
 
 + 2.obj.toJson()
 
 + 3.obj.toYaml()


# json

  +  json.dumps(dict)  //字典转字符串
  
  + json.loads(string) //字符串转字典
  
  + json.dump(json_info,file)   //将json信息写进文件
  
  + file=open('x.json', 'r', encoding='utf-8')
     ----json.load(file)    //读取json信息
