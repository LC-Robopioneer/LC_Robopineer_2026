Motor_Test 分支 - LC_Robopineer_2026本项目是 LC_Robopineer 战队针对 RoboMaster 2026 赛季 开发的下位机控制系统。
Motor_Test 分支专注于底层电机驱动的验证与性能调优。
📁 目录结构说明项目采用模块化设计，各文件夹定义如下：目录名称功能描述核心内容
+ User_alg 算法层PID 控制器、滤波器、逆解算、大疆/达妙电机转换公式。
+ User_chariot 机器人配置整车参数定义，如轮距、轴距、电机 ID 分配。
+ User_drv 底层驱动HAL 库封装，包括 CAN、FDCAN、UART、SPI (DWT) 等。
+ User_dvc 设备层电机对象（M3508, M2006, GM6020, 宇树, 达妙）、遥控器。
+ User_ita 交互/接口协议解析、数据转发、底层与逻辑层的映射。User_tsk任务层FreeRTOS 任务（电机控制环、通信任务、系统监控）。
