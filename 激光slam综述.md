## slam是什么？
* Location:在给定地图的情况下，估计机器人的位姿。
* Mapping:在给定机器人位姿的情况下，估计环境地图。
* SLAM (simultaneous localization and mapping)同步定位（估计机器人的位姿）与建图（环境地图）

## 3D激光slam的后端
* Filter-based SLAM 以扩展卡尔曼滤波（EKF）为代表的滤波方法 （老古董了）
* Graph-based SLAM 图优化方法，非线性优化

## 3D激光slam的传感器
* IMU(惯性测量单元)
* Wheel Odometry（轮式里程计）
* Lidar（激光雷达）

## 3D激光slam帧间匹配算法
* Point-to-Plane ICP
* NDT(Normal Distribution Transfomation)
* Feature-based Method

## 3D激光slam回环检测
* Scan-to-Scan
* Scan-to-Map
* Branch and Bound & Lazy Decision

## 3D激光SLAM的发展
* LOAM - 纯激光，匀速运动假设，无回环
* V-LOAM - 视觉激光融合，漂移匀速假设，无回环
* VElO - 视觉激光融合，无运动畸变假设，有回环

## 3D激光SLAM中的问题
* 1、退化环境(Degeneration Environment)
* 2、地图的动态更新(Map Update)
* 3、全局定位(Global Localization)
* 4、动态环境定位(Dynamic Localization)