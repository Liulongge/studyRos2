$ mkdir demo
$ cd demo
$ mkdir src

1.创建package
编译类型：ament_cmake
node名：node1
package名：package1

$ ros2 pkg create --build-type ament_cmake --node-name node1 package1

2.编译
$ cd demo
$ colcon build

3.想要使用自定义包\节点，需要 source工作区安装文件，否则无法使用
$ source install/setup.sh 

4.运行
$ ros2 run package1 node1

5.修改xml信息