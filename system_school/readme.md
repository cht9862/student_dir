## 1-需求分析
    - 管理员试图
        1. 注册
        2. 登录
        3. 创建学校
        4. 创建课程（先选择学校）
        5. 创建讲师 

    - 学员视图
        1. 注册
        2. 登录
        3. 选择校区
        4. 选择课程（先选择校区）
            - 学生选择课程，课程也选择学生
        5. 查看分数
        
    - 讲师视图
        1. 登录
        2. 教授课程    
        3. 选择教授课程
        4. 查看课程下学生
        5. 修改学生分数


## 2-程序的架构设计
    - 三层架构
        1. 用户层
            用来与用户进行交互的
            逻辑判断，注册功能中的两次密码是否一致校验
            core 
                -src.py   #主视图
                -admin.py
                    -admin_view
                -student.py
                    -student_view
                -teacher.py
                    -teacher_view
        2. 逻辑接口层
            核心业务逻辑的处理
            interface
                admin_inter
                student_inter
                teacher_inter
        3.数据处理层
            做数据的处理，数据的增删改查
            db
                db_handler.py
                models.py
## 3-任务开发
## 4-测试
## 5-上线