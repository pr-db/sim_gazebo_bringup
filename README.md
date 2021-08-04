<h1>Introduction to Gazebo </h1>
<h3>WHY GAZEBO?</h3>
</br><img src="https://gblobscdn.gitbook.com/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXaIxqcmP2grIz5ToTW%2F-MXaND_w1UbqoGHP4VNv%2Fgazebo.png?alt=media&token=a05f7459-89f1-454a-a581-59ea9da22411" alt="W3Schools.com" width="420" height="540"> 
<p>Gazebo is a full-fledged simulation environment that is compatible with PX4. In 2021, NXP Cup contestants may use the Gazebo simulation for an extra challenge at home. The benefit to using the Gazebo simulation environment is that you can test your code without crashing or damaging your actual NXP Cup car. The code modules that you run on your actual NXP Cup car can be ported to the Gazebo simulation environment with ease - and if you're using a brushless Cup car, you'll essentially be running the same exact code.<p>
<h3>Installing ROS2</h3>
<h4>You need to download this file inorder to install the ROS</h4>
</br>
<a href="https://firebasestorage.googleapis.com/v0/b/gitbook-28427.appspot.com/o/assets%2F-MWeiLnwrIKZJWLFsXhf%2F-MXcfaeFblmznqth_0fk%2F-MXcgSRrBPzq5-K6O-C5%2Ffoxy_install_aim.sh?alt=media&token=2adf3a55-8463-4ff1-890e-67b6d32fe747">Download this file</a>
</br>
</br>RUN THE FOLLOWING COMMANDS
</br>cd ~/Downloads
</br>chmod a+x foxy_install_aim.sh
</br>./foxy_install_aim.sh
</br>source ~/.bashrc
# Installing Robocon Gazebo
</br>cd ~
</br>mkdir -p robocon_ws/src && cd robocon_ws/src
</br>git clone https://github.com/pr-db/sim_gazebo_bringup.git -b aim
</br>cd ~/robocon_ws
</br>colcon build --packages-select sim_gazebo_bringup --symlink-install
</br>echo "source /home/$USER/robocon_ws/install/setup.bash" >> ~/.bashrc
</br>source ~/.bashrc
</br>ros2 launch sim_gazebo_bringup sim_gazebo.launch.py
