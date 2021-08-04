<h1>Robocon Gazebo </h1>
<div class="gazebo">
<h3 display: block;>WHY GAZEBO?</h3>
<p align="center">
</br><img src="https://gblobscdn.gitbook.com/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXaIxqcmP2grIz5ToTW%2F-MXaND_w1UbqoGHP4VNv%2Fgazebo.png?alt=media&token=a05f7459-89f1-454a-a581-59ea9da22411" width="687" height="319"> 
</p>
<p>Gazebo is a full-fledged simulation environment that offers the ability to accurately and efficiently simulate populations of robots in complex indoor and outdoor environments. </p>
</div>
<div class="installation">
<h3 display: block;>Installing ROS2 Foxy Fitzroy</h3>
<h5>Download ROS2 Foxy using the link below</h4>
<a href="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXcfaeFblmznqth_0fk%2F-MXcgSRrBPzq5-K6O-C5%2Ffoxy_install_aim.sh?alt=media&token=2adf3a55-8463-4ff1-890e-67b6d32fe747">download</a>
  <p></p>
  <h5>Run the following commands after the download</h5>
<ul display: block; style="font-family:verdana">
  <li>cd ~/Downloads</li>
  <li>chmod a+x foxy_install_aim.sh</li>
  <li>./foxy_install_aim.sh</li>
  <li>source ~/.bashrc</li>
</ul>
</div>
<div class="robocon">
<h3 display: block;>Installing Robocon Gazebo</h3>
 <ul display:block;style="font-family:verdana">
    <li>cd ~</li>
    <li>mkdir -p robocon_ws/src && cd robocon_ws/src</li>
    <li>git clone https://github.com/pr-db/sim_gazebo_bringup.git -b aim</li>
    <li>cd ~/robocon_ws</li>
    <li>colcon build --packages-select sim_gazebo_bringup --symlink-install</li>
    <li>echo "source /home/$USER/robocon_ws/install/setup.bash" >> ~/.bashrc</li>
    <li>source ~/.bashrc</li>
    <li>ros2 launch sim_gazebo_bringup sim_gazebo.launch.py</li>
   </ul>
</div>
