# UTS-Turtlebot4-MultiPoint-Navigation
RE702 Midterm Exam 4222201043 Ricard Riovaldo Simatupang RE 7B Pagi


## Multi Point Autonomous-and-Localization-Turtlebot-4
Repositori ini disusun untuk memenuhi tugas Ujian Tengah Semester pada mata kuliah Lokalisasi dan Pemetaan (RE702). Paket ROS2 ini berfungsi untuk mengarahkan TurtleBot4 berpindah dari satu titik ke titik lainnya serta mengaktifkan buzzer sesuai ketentuan asesmen.

## Multi Point Autonomous-and-Localization-Turtlebot-4
Sebelum melakukan proses build dan menjalankan package ROS2 ini, pastikan Anda telah membuat peta yang sesuai dengan environment yang digunakan. Peta hasil pemetaan harus disimpan di folder maps/. Untuk membuat peta baru, Anda dapat mengikuti panduan resmi TurtleBot4:
https://turtlebot.github.io/turtlebot4-user-manual/tutorials/generate_map.html
Pastikan laptop atau PC berada pada jaringan LAN atau WiFi yang sama dengan TurtleBot4, lalu lakukan koneksi SSH ke robot.

## 1. Run Turtlebot-4 Navigation Localization
Run TurtleBot4, Command:
```bash
ros2 launch turtlebot4_navigation localization.launch.py map:=path/ke/map.yaml
```
## 2. Run Nav2 TurtleBot4
Run TurtleBot4, Command:
```bash
ros2 launch turtlebot4_navigation nav2.launch.py
```
## 3. Run RViz2 (On laptop or PC)
Run TurtleBot4, Command:
```bash
=ros2 launch turtlebot4_viz view_navigation.launch.py
```

### Navigation Setup Completed


# How to Build the Package in This Repository
Create ROS2 workspace:
```bash
mkdir -p ros2_ws/src
cd ros2_ws/src
```

Clone This repository:
```bash
https://github.com/Glbaymax37/UTS-Turtlebot4-MultiPoint.git
```

Build Using
```bash
cd ../
colcon build
source install/setup.bash
```

Running Program
```bash
ros2 run abdi_pkg abdinode
```

# DEMO Video

[![Demo Video](https://img.youtube.com/vi/b6Jc3NDo4qI/0.jpg)](https://youtu.be/b6Jc3NDo4qI)





