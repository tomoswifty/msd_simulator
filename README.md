# MSD simulator for tunnel inspection 
```
version 
os : ubuntu 20.0.4
ros : noetic
```
`/robot` にCADからのSTLファイルと色，座標を修正したblenderのファイルを保存．

Save the STL file from CAD and the blender file with corrected colors and coordinates to `/robot`.

## シミュレータの起動  Starting the Simulator
シミュレータのみの起動
```bash:msd_tunnel_sim.launch
roslaunch msd_simulator msd_tunnel_dtw.launch
```

シミュレータとRvizの起動
![](/picture/simulator.png)
```
roslaunch msd_simulator msd_tunnel_gazebo_rviz.launch
```

センサーシミュレーション

rplidar s1と超音波センサをシミュレーション
![](/picture/rplidars1_sim.png)
```
roslaunch msd_simulator msd_tunnel_sensor.launch
```

キーボードコントローラ
```
roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
```
