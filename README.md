# openDog_Leg

<?xml version="1.0"?>
<robot name = "opendog">

<!-- CTRL + Backslash to comment -->
<!-- Child's COG is referenced from the parent's origin -->

<!-- gazebo plugins go here -->
    <gazebo>
        <plugin name="gazebo_ros_control" filename="libgazebo_ros_control.so">
            <robotNamespace>/opendog</robotNamespace>
        </plugin>
    </gazebo>

 <material name="blue">
        <color rgba="0 0 0.8 1"/>
    </material>

    <material name="red">
        <color rgba="0.8 0 0 1"/>
    </material>

    <material name="green">
        <color rgba="0 0.8 0 1"/>
    </material>

    <material name="grey">
        <color rgba="0.75 0.75 0.75 1"/>
    </material>

    <material name="white">
        <color rgba="1.0 1.0 1.0 1"/>
    </material>

    <material name="black">
        <color rgba="0 0 0 1"/>
    </material>


    <link name = "openDog_body">
     <visual>
       <origin xyz = "0 0 0.7" rpy = "0 0 0"/>
       <geometry>
         <box size = "0.31 0.881 0.195"/>
       </geometry>
       <material name = "blue"/>
     </visual>
        <collision>
            <origin xyz = "0 0 0.7" rpy = "0 0 0"/>
            <geometry>
                <box size = "0.31 0.881 0.195"/>
            </geometry>
        </collision>
        <!-- <inertial>
       <origin xyz = "0 0 0.7" rpy = "0 0 0"/>
    <mass value="1"/>
      <inertia
        ixx="1.0" ixy="0.0" ixz="0.0"
        iyy="1.0" iyz="0.0"
        izz="1.0"/>
    </inertial> -->
    </link>

    <link name = "dummy_mass">
        <visual>
            <origin xyz = "0 0 0" rpy = "0 0 0"/>
            <geometry>
                <box size = "0.31 0.881 0.195 "/>
            </geometry>
            <material name = "black"/>
        </visual>
        <collision>
            <origin xyz = "0 0 0" rpy = "0 0 0"/>
            <geometry>
                <box size = "0.31 0.881 0.195"/>
            </geometry>
        </collision>
        <inertial>
       <origin xyz = "0 0 0.7" rpy = "0 0 0"/>
    <mass value="24.326"/>
      <inertia
        ixx="2.44310079067" ixy="0.0" ixz="0.0"
        iyy="0.402464416667" iyz="0.0"
        izz="2.61736450733"/>
    </inertial>
    </link>

    <link name = "hip_tube_1">
     <visual>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
       <geometry>
         <cylinder length = "0.165" radius = "0.05715"/>
       </geometry>
       <material name = "green"/>
     </visual>
        <collision>
            <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
            <geometry>
                <cylinder length = "0.165" radius = "0.05715"/>
            </geometry>
        </collision>
        <inertial>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
    <mass value="1"/>
      <inertia
        ixx="1.0" ixy="0.0" ixz="0.0"
        iyy="1.0" iyz="0.0"
        izz="1.0"/>
    </inertial>
    </link>

    <link name = "hip_tube_2">
     <visual>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
       <geometry>
         <cylinder length = "0.165" radius = "0.05715"/>
       </geometry>
       <material name = "green"/>
     </visual>
        <collision>
            <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
            <geometry>
                <cylinder length = "0.165" radius = "0.05715"/>
            </geometry>
        </collision>
        <inertial>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
    <mass value="1"/>
      <inertia
        ixx="1.0" ixy="0.0" ixz="0.0"
        iyy="1.0" iyz="0.0"
        izz="1.0"/>
    </inertial>
    </link>

    <link name = "hip_tube_3">
     <visual>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
       <geometry>
         <cylinder length = "0.165" radius = "0.05715"/>
       </geometry>
       <material name = "green"/>
     </visual>
        <collision>
            <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
            <geometry>
                <cylinder length = "0.165" radius = "0.05715"/>
            </geometry>
        </collision>
        <inertial>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
    <mass value="1"/>
      <inertia
        ixx="1.0" ixy="0.0" ixz="0.0"
        iyy="1.0" iyz="0.0"
        izz="1.0"/>
    </inertial>
    </link>

    <link name = "hip_tube_4">
     <visual>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
       <geometry>
         <cylinder length = "0.165" radius = "0.05715"/>
       </geometry>
       <material name = "green"/>
     </visual>
        <collision>
            <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
            <geometry>
                <cylinder length = "0.165" radius = "0.05715"/>
            </geometry>
        </collision>
        <inertial>
       <origin xyz = "0.0 0.0 0.0" rpy = "0 1.5708 0"/>
    <mass value="1"/>
      <inertia
        ixx="1.0" ixy="0.0" ixz="0.0"
        iyy="1.0" iyz="0.0"
        izz="1.0"/>
    </inertial>
    </link>







 <link name = "lower_extrusion_leg1">
   <visual>
     <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
     <geometry>
       <box size = "0.02 0.04 0.31"/>
     </geometry>
     <material name = "grey"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
            <geometry>
                <box size = "0.02 0.04 0.31"/>
            </geometry>
        </collision>
        <inertial>
        <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
    <mass value="2.224"/>
      <inertia
        ixx="0.01566066666667" ixy="0.0" ixz="0.0"
        iyy="0.0156050666667" iyz="0.0"
        izz="9.26666666667e-05"/>
    </inertial>
 </link>

 <link name = "lower_extrusion_leg2">
   <visual>
     <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
     <geometry>
       <box size = "0.02 0.04 0.31"/>
     </geometry>
     <material name = "grey"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
            <geometry>
                <box size = "0.02 0.04 0.31"/>
            </geometry>

        </collision>
        <inertial>
        <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
    <mass value="2.224"/>
      <inertia
        ixx="0.01566066666667" ixy="0.0" ixz="0.0"
        iyy="0.0156050666667" iyz="0.0"
        izz="9.26666666667e-05"/>
    </inertial>

 </link>

 <link name = "lower_extrusion_leg3">
   <visual>
     <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
     <geometry>
       <box size = "0.02 0.04 0.31"/>
     </geometry>
     <material name = "grey"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
            <geometry>
                <box size = "0.02 0.04 0.31"/>
            </geometry>
        </collision>
        <inertial>
        <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
    <mass value="2.224"/>
      <inertia
        ixx="0.01566066666667" ixy="0.0" ixz="0.0"
        iyy="0.0156050666667" iyz="0.0"
        izz="9.26666666667e-05"/>
    </inertial>
 </link>

 <link name = "lower_extrusion_leg4">
   <visual>
     <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
     <geometry>
       <box size = "0.02 0.04 0.31"/>
     </geometry>
     <material name = "grey"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
            <geometry>
                <box size = "0.02 0.04 0.31"/>
            </geometry>
        </collision>
        <inertial>
    <origin xyz = "0.0 0.155 0.0" rpy = "1.5708 3.14 0"/>
    <mass value="2.224"/>
      <inertia
        ixx="0.01566066666667" ixy="0.0" ixz="0.0"
        iyy="0.0156050666667" iyz="0.0"
        izz="9.26666666667e-05"/>
    </inertial>
 </link>


 <link name = "upper_extrusion_leg1">
   <visual>
     <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
     <geometry>
       <box size = "0.02 0.06 0.39"/>
     </geometry>
     <material name = "red"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
            <geometry>
                <box size = "0.02 0.06 0.39"/>
            </geometry>
            <material name = "red"/>
        </collision>
        <inertial>
    <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
    <mass value="4.036"/>
      <inertia
        ixx="0.013091775" ixy="0.0" ixz="0.0"
        iyy="0.000336333333333" iyz="0.0"
        izz="0.0128227083333"/>
    </inertial>
 </link>

 <link name = "upper_extrusion_leg2">
   <visual>
     <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
     <geometry>
       <box size = "0.02 0.06 0.39"/>
     </geometry>
     <material name = "red"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
            <geometry>
                <box size = "0.02 0.06 0.39"/>
            </geometry>
            <material name = "red"/>
        </collision>
        <inertial>
    <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
    <mass value="4.036"/>
      <inertia
        ixx="0.013091775" ixy="0.0" ixz="0.0"
        iyy="0.000336333333333" iyz="0.0"
        izz="0.0128227083333"/>
    </inertial>
 </link>

 <link name = "upper_extrusion_leg3">
   <visual>
     <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
     <geometry>
       <box size = "0.02 0.06 0.39"/>
     </geometry>
     <material name = "red"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
            <geometry>
                <box size = "0.02 0.06 0.39"/>
            </geometry>
            <material name = "red"/>
        </collision>
        <inertial>
    <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
    <mass value="4.036"/>
      <inertia
        ixx="0.013091775" ixy="0.0" ixz="0.0"
        iyy="0.000336333333333" iyz="0.0"
        izz="0.0128227083333"/>
    </inertial>
 </link>


 <link name = "upper_extrusion_leg4">
   <visual>
     <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
     <geometry>
       <box size = "0.02 0.06 0.39"/>
     </geometry>
     <material name = "red"/>
   </visual>
        <collision>
            <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
            <geometry>
                <box size = "0.02 0.06 0.39"/>
            </geometry>
            <material name = "red"/>
        </collision>
    <inertial>
    <origin xyz = "0.0 0.195 0.0" rpy = "1.5708 0 0"/>
    <mass value="4.036"/>
      <inertia
        ixx="0.013091775" ixy="0.0" ixz="0.0"
        iyy="0.000336333333333" iyz="0.0"
        izz="0.0128227083333"/>
    </inertial>
  </link>

<!-- knee links  -->
  <link name = "knee1">
    <visual>
      <collision>
        <origin xyz = "" rpy = ""/>
        <geometry>
          <box size = ".04 0.0303 .13"/>
          </geometry>
          <material name = "red"/>
        </collision>
    <inertial>
    <origin xyz = "" rpy = ""/>
    <!-- mass value in kg -->
    <mass value="187.164"/>
    <inertia
      ixx="" ixy="" ixz=""
      iyy="" iyz=""
      izz=""/>
    </inertial>
 </link>

 <link name = "knee2">
   <visual>
     <collision>
       <origin xyz = "" rpy = ""/>
       <geometry>
         <box size = ".04 0.0303 .13"/>
         </geometry>
         <material name = "red"/>
       </collision>
   <inertial>
   <origin xyz = "" rpy = ""/>
   <!-- mass value in kg -->
   <mass value="187.164"/>
   <inertia
     ixx="" ixy="" ixz=""
     iyy="" iyz=""
     izz=""/>
   </inertial>
</link>

<link name = "knee3">
  <visual>
    <collision>
      <origin xyz = "" rpy = ""/>
      <geometry>
        <box size = ".04 0.0303 .13"/>
        </geometry>
        <material name = "red"/>
      </collision>
  <inertial>
  <origin xyz = "" rpy = ""/>
  <!-- mass value in kg -->
  <mass value="187.164"/>
  <inertia
    ixx="" ixy="" ixz=""
    iyy="" iyz=""
    izz=""/>
  </inertial>
</link>

<link name = "knee4">
  <visual>
    <collision>
      <origin xyz = "" rpy = ""/>
      <geometry>
        <box size = ".04 0.0303 .13"/>
        </geometry>
        <material name = "red"/>
      </collision>
  <inertial>
  <origin xyz = "" rpy = ""/>
  <!-- mass value in kg -->
  <mass value="187.164"/>
  <inertia
    ixx="" ixy="" ixz=""
    iyy="" iyz=""
    izz=""/>
  </inertial>
</link>

    <joint name = "dummy_joint" type = "fixed">
        <parent link = "openDog_body"/>
        <child link  = "dummy_mass"/>
        <origin xyz = "0 0 0.7" rpy = "0 0 0"/>
    </joint>

    <joint name="hip_joint_1" type="fixed">
        <parent link="openDog_body"/>
        <child link="hip_tube_1"/>
        <origin xyz="-0.226 0.2825 0.7" rpy="0 0 0"/>
    </joint>

    <joint name="hip_joint_2" type="fixed">
        <parent link="openDog_body"/>
        <child link="hip_tube_2"/>
        <origin xyz="0.226 0.2825 0.7" rpy="0 0 0"/>
    </joint>

    <joint name="hip_joint_3" type="fixed">
        <parent link="openDog_body"/>
        <child link="hip_tube_3"/>
        <origin xyz="-0.226 -0.2825 0.7" rpy="0 0 0"/>
    </joint>

    <joint name="hip_joint_4" type="fixed">
        <parent link="openDog_body"/>
        <child link="hip_tube_4"/>
        <origin xyz="0.226 -0.2825 0.7" rpy="0 0 0"/>
    </joint>

    <joint name="femur_joint1" type="revolute">
        <parent link="hip_tube_1"/>
        <child link="upper_extrusion_leg1"/>
        <origin xyz="-0.05 0 0" rpy="1.5708 -3.14 1.5708"/>
        <limit lower="-1.579" upper="-0.567" effort="5000" velocity="1.0"/>
        <axis xyz="0 0 1"/>
    </joint>

    <transmission name="simple_trans0">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="femur_joint1">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_1">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>


    <joint name="femur_joint2" type="revolute">
        <parent link="hip_tube_2"/>
        <child link="upper_extrusion_leg2"/>
        <origin xyz="0.05 0 0" rpy="1.5708 -3.14 1.5708"/>
        <limit lower="-1.579" upper="-0.567" effort="5000" velocity="1.0"/>
        <axis xyz="0 0 1"/>
    </joint>

    <transmission name="simple_trans1">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="femur_joint2">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_2">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>

    <joint name="femur_joint3" type="revolute">
        <parent link="hip_tube_3"/>
        <child link="upper_extrusion_leg3"/>
        <origin xyz="-0.05 0 0" rpy="1.5708 -3.14 1.5708"/>
        <limit lower="-1.579" upper="-0.567" effort="5000" velocity="1.0"/>
        <axis xyz="0 0 1"/>
    </joint>

    <transmission name="simple_trans2">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="femur_joint3">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_3">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>

    <joint name="femur_joint4" type="revolute">
        <parent link="hip_tube_4"/>
        <child link="upper_extrusion_leg4"/>
        <origin xyz="0.05 0 0" rpy="1.5708 -3.14 1.5708"/>
        <limit lower="-1.579" upper="-0.567" effort="5000" velocity="1.0"/>
        <axis xyz="0 0 1"/>
    </joint>

    <transmission name="simple_trans3">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="femur_joint4">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_4">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>

    <joint name = "knee_joint_leg1" type = "revolute">
        <parent link = "upper_extrusion_leg1"/>
        <child link = "lower_extrusion_leg1"/>
        <origin xyz="0 0.39 0" rpy="0 0 0"/>

        <limit effort="5000"  lower="1.352" upper="2.8715" velocity="1.0"/>
        <axis xyz="0 0 1"/>

    </joint>

    <transmission name="simple_trans4">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="knee_joint_leg1">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_5">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>

    <joint name = "knee_joint_leg2" type = "revolute">
        <parent link = "upper_extrusion_leg2"/>
        <child link = "lower_extrusion_leg2"/>
        <origin xyz="0 0.39 0" rpy="0 0 0"/>
        <limit effort="5000"  lower="1.352" upper="2.8715" velocity="1.0"/>
        <axis xyz="0 0 1"/>

    </joint>

    <transmission name="simple_trans5">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="knee_joint_leg2">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_6">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>

    <joint name = "knee_joint_leg3" type = "revolute">
        <parent link = "upper_extrusion_leg3"/>
        <child link = "lower_extrusion_leg3"/>
        <origin xyz="0 0.39 0" rpy="0 0 0"/>
        <limit effort="5000"  lower="1.352" upper="2.8715" velocity="1.0"/>
        <axis xyz="0 0 1"/>
    </joint>

    <transmission name="simple_trans6">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="knee_joint_leg3">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_7">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>



    <joint name = "knee_joint_leg4" type = "revolute">
        <parent link = "upper_extrusion_leg4"/>
        <child link = "lower_extrusion_leg4"/>
        <origin xyz="0 0.39 0" rpy="0 0 0 "/>
        <limit effort="5000"  lower="1.352" upper="2.8715" velocity="1.0"/>
        <axis xyz="0 0 1"/>
    </joint>

    <transmission name="simple_trans7">
  <type>transmission_interface/SimpleTransmission</type>
  <joint name="knee_joint_leg4">
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </joint>
  <actuator name="motor_8">
    <mechanicalReduction>1</mechanicalReduction>
    <hardwareInterface>hardware_interface/EffortJointInterface</hardwareInterface>
  </actuator>
</transmission>


</robot>
