# Djet
##Attention:

####测试地址：http://127.0.0.1:8000/crud/web02/userinfo/

###适用于Django2.0,如果你的版本低于2.0,请自行修改！！！比如：url中的path,namespace等！

####主要根据Django源码搭建的组件，对model模型类中的数据进行快速的增删改查，同时增加了一些新功能比如可以根据条件跳回原页面

update-log:

2017-12-29 增加自定制ModelForm,自定制排序配置

2017-12-29 增加搜索框，可以根据搜索条件进行搜索

2017-12-30 增加批量处理，，可以批量处理数据，修改部分bug

2018-01-01 增加综合搜索功能及指定了to_field处理方式

2018-01-01 增加外键多对多功能popup添加方式，修复部分bug

#### HOW TO USE IT:

    在web02的crud文件注册models中的类，Example:
    
    class UserInfoConfig(CrudConfig):
    
    """必须继承CrudConfig"""
    
        list_display=['字段']
        
    service.site.regiser(UserInfo, UserInfoConfig)
    
    更多用法详见代码！
    

