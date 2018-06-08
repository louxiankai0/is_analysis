# 接口：chooseCourse  [返回](../README.md)
用例： [选择课程](../用例/选择课程.md)

- 功能：
    老师和学生进行选课。
    
- 权限：    
    老师/学生。
    
- API请求地址： 
     http://202.115.82.8:1522/v1/api/chooseCourse/

- 请求方式 ：
    GET

- 请求参数说明:        

  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|
  |term_ID|学期ID，确认学期|
  |course_ID|课程ID|
  |course_name|课程名称|
  |course_PLACE|课程地点|
  |course_PEOPLE|课程人数|
  
    
- 返回实例：

        {         
            "status": true,
            "info": null,    
            "course_ID": "04450280"
            "course_name": "信息系统分析与设计"
            "course_PLACE": "10417"
            "course_PEOPLE": "60"
        }
 
- 返回参数说明：    
 
  |参数名称|说明|
  |:---------:|:--------------------------------------------------------|      
  |status|bool类型，true表示正确的返回，false表示有错误|
  |info|返回结果说明信息|
  |term_ID|学期ID，确认学期|
  |course_ID|课程ID|
  |course_name|课程名称|
  |course_PLACE|课程地点|
  |course_PEOPLE|课程人数|

