# 可用性测试



## 可用性指标

### Effectiveness

用户能不能完成任务？

计算方式：

## Efficiency

用户完成任务的效率

## 满意度

用户完成任务后的满意程度



## 可用性实验

### 实验流程


1. Develop the Test Plan
2. Setup a testing environment
3. Find and select participants
4. Prepare test materials
5. Conduct the test sessions
6. Debrief the participant and observers
7. Analyze data and observations
8. Report findings and recommendations

#### 测试计划
- Purpose, goals and objectives of the test
- Research questions
- Participant characteristics
- Method
- Task list
- Test environment, equipment, and logistics
- Test moderator role
- Data to be collected and evaluation measures
- Report contents and presentation


## Sphinx 文档可用性测试

### 环境准备

1. 使用腾讯会议录制桌面与人像
2. 使用 [Usability Test Data Logger tool v5.1.1](https://www.userfocus.co.uk/resources/datalogger.html) 记录与分析数据



### 测试任务

1. 安装sphinx。成功标志：

   ```
    $ sphinx-quickstart --version
    sphinx-quickstart 4.0.1
   ```

   

2. 写一个rST文件 (Title, Section Title, Bold)
3. 将整个项目发布为 html 站点



### 分析结果

1. 使用 UTDL 登录各测试数据
2. 观察视频，观察其中用户完成任务的过程中遇到的问题
3. 数据结果的分析并用于文档的改进
