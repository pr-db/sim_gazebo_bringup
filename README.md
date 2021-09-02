<h1>Robo Simulation </h1>
<div class="Gazebo">
<h2 display: block;>Ros and Gazebo</h2>
<p align="center">
</br>
<img src="https://miro.medium.com/max/680/1*n4TxKdA4LeMTn95m6ogisQ.png"  width="460" height="212">
<img src="https://gblobscdn.gitbook.com/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXaIxqcmP2grIz5ToTW%2F-MXaND_w1UbqoGHP4VNv%2Fgazebo.png?alt=media&token=a05f7459-89f1-454a-a581-59ea9da22411" width="460" height="212"> 

</p>
<p>Robot Operating System (ROS) is an open-source robotics middleware suite. ROS is a collection of software frameworks for robot software development, it provides services for hardware abstraction, low-level device control, message-passing between processes, and package management.Gazebo is a full-fledged simulation environment that offers the ability to accurately and efficiently simulate populations of robots in complex indoor and outdoor environments. </p>
</div>
<div class="installation">
<h3 display: block;>Installing ROS2 Foxy Fitzroy</h3>
<a href="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXcfaeFblmznqth_0fk%2F-MXcgSRrBPzq5-K6O-C5%2Ffoxy_install_aim.sh?alt=media&token=2adf3a55-8463-4ff1-890e-67b6d32fe747">Download ROS2 Foxy</a>
  <p></p>
  <h5>Run the following commands after the download</h5>
<ul display: block; style="font-family:verdana">
  <li>cd ~/Downloads</li>
  <li>chmod a+x foxy_install_aim.sh</li>
  <li>./foxy_install_aim.sh</li>
  <li>source ~/.bashrc</li>
</ul>
</div>
<div class="robo">
<h3 display: block;>Installing Robo Gazebo</h3>
 <ul display:block;style="font-family:verdana">
    <li>cd ~</li>
    <li>mkdir -p ros2ws/src && cd ros2ws/src</li>
    <li>git clone https://github.com/pr-db/sim_gazebo_bringup.git -b mini</li>
    <li>cd ~/ros2ws</li>
    <li>colcon build --packages-select sim_gazebo_bringup --symlink-install</li>
    <li>echo "source /home/$USER/ros2ws/install/setup.bash" >> ~/.bashrc</li>
    <li>source ~/.bashrc</li>
    <li>ros2 launch sim_gazebo_bringup sim_gazebo.launch.py</li>
   </ul>
  <p>After running the above command you will be asked to run few commands. Copy them and run them before moving to next step</p>

<h3 display: block;>Running Robo Simulation</h3>
  <p> You've successfully installed Robo Gazebo! For the siulation, run the command below</p>
 <ul display:block;style="font-family:verdana">
   <li>ros2 launch sim_gazebo_bringup sim_gazebo.launch.py</li>



</div>
