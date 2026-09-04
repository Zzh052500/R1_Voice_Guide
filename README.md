先进入仿真容器
cd /home/maxw/4sim/gh-ref/tour-guide-robot/tour-guide-robot/docker_stuff/docker_sim_compose
./run_sim.sh
再开一个终端
maxw@5080-MS-eSport-Z890M:~/4sim/gh-ref/tour-guide-robot/tour-guide-robot/docker_stuff/docker_sim_compose$ TOUR_CONTAINER=docker_sim_compose-sim-run-a255cef5fab0   /home/maxw/r1_vioce_contol/r1_voice_control.sh --ensure-stack 
进入到agents启动才算成功启动
脚本已经放在/home/max/r1_vioce_contoll
如果要可视化的话还是要启动RViz、Gazebo、Nav2 和 YARP navigation 端口
回到容器内
./sim_up.sh
在 yarpmanager 中先启动导航最小控制集：
Navigation_ROS2_R1Mk3_SIM_light
就可以可视化了。
