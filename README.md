# 前言

实验室排课系统是一个针对高校实验室资源进行有效管理、提高排课效率的在线系统。本项目是基于SSM（Spring、SpringMVC、MyBatis）框架开发的实验室排课系统，旨在为实验室管理人员和教师提供一个便捷、高效的排课工具。

# 内容介绍

本项目主要实现了以下功能：

1. 用户登录与权限管理：根据用户角色（如实验室管理员、教师、学生等）进行权限控制，保障系统安全。
2. 实验室信息管理：实现对实验室的基本信息（如实验室名称、地点、设备等）进行维护。
3. 课程信息管理：实现对课程的基本信息（如课程名称、学分、授课教师等）进行维护。
4. 排课功能：根据实验室资源和课程需求，自动生成排课表，实现课程与实验室的高效匹配。
5. 课程查询与调整：教师和学生可查询个人课表，教师可进行调课操作。

# 技术介绍

- 语言：Java
- 使用框架：Spring、SpringMVC、MyBatis
- 前端技术：JS、Vue、CSS3
- 开发工具：IDEA/Eclipse
- 数据库：MySQL 5.7/8.0
- 数据库管理工具：phpstudy/Navicat
- JDK版本：jdk1.8
- Maven: apache-maven 3.8.1-bin
- 前端环境：Node.Js 12\14\16

# 核心代码

以下是项目中的一段核心代码，展示了如何实现课程信息的查询：

```java
// CourseMapper.xml
<select id="findCourseList" resultType="Course">
    SELECT * FROM course
    <where>
        <if test="courseName != null and courseName != ''">
            AND course_name LIKE CONCAT('%', #{courseName}, '%')
        </if>
        <if test="teacherId != null">
            AND teacher_id = #{teacherId}
        </if>
    </where>
</select>

// CourseService.java
public List<Course> findCourseList(Map<String, Object> params) {
    return courseMapper.findCourseList(params);
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img10.360buyimg.com/ddimg/jfs/t1/334228/18/8790/139067/68b88008Ff01136fe/d9be16958db4aba5.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/324989/19/15671/72695/68b87fdfFc6b583d0/6edc5cd852f2aa33.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/332459/21/8486/72507/68b87fdfFccfc116d/3427f22530924d99.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/326830/19/15393/54229/68b87fe0Fad2fc35e/f2134eb082fb49b1.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/293627/26/23890/55742/68b87fe1Fb536da40/9c02756461bff24f.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/326299/23/15159/56907/68b87fe1Ff9566ef3/d52e7ecb83bfe3ff.jpg)

![介绍图片](https://img11.360buyimg.com/ddimg/jfs/t1/328028/16/15358/50192/68b87fe2F821a8630/541362f9b6ce260e.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/339598/1/6288/56759/68b87fe3F675b8e6e/4796687a9c09873f.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/329873/20/8915/62164/68b87fe3F10e5d1c5/22523997dd88dd2f.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/340209/36/6285/53910/68b87fe4Fd23fc438/ccfef45bda4c1c39.jpg)
