रॉस औपरेटिंग सिस्टम के ऊपर बनी एक परत की तरह है जो रोबोटों के लिये क्रमादेश बनाना आसान बनाती है। 
![परत](/assets/ros.png)

एक रोबोट के अलग-अलग भागों में अलग-अलग क्रमादेश (**नोड**) काम करते हैं। एक (या एक से अधिक) नोड के क्रमादेश एक पैकेज बनाते हैं। रॉस पर काम करते वक्त हम एक वर्कस्पेस में काम करते हैं जिसमें एक से ज्यादा पैकेज एक साथ हो सकते हैं। उदाहरण के लिये हो सकता है कि रोबोट में देखने वाली एक नोड हो, छूने वाली दूसरी, उठाने वाली तीसरी और इन सबके क्रमादेश अपने-अपने पैकेज में होंगे। नीचे दिये गये कमांड मिलकर एक खाली वर्कसेपेस बनाते हैं।

![नोड](/assets/ros-2.png)

**वर्कस्पेस बनाना**
```bash
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/
$ catkin_make -DPYTHON_EXECUTABLE=/usr/bin/python3
$ ls
build devel src
$ source devel/setup.sh
$ echo $ROS_PACKAGE_PATH
/home/hgarg/catkin_ws/src:/opt/ros/kinetic/share
```
**पैकेज बनाना**
```bash
$ cd ~/catkin_ws/src
$ catkin_create_pkg my_publisher rospy
Created file my_publisher/package.xml
Created file my_publisher/CMakeLists.txt
Created folder my_publisher/src
Successfully created files in /home/hgarg/catkin_ws/src/my_publisher. Please adjust the values in package.xml.
hgarg@hgarg-OptiPlex-3046:~/catkin_ws/src$ ls my_publisher/
CMakeLists.txt  package.xml  src

```
ये अलग-अलग नोड आपस में मैसेजों के जरिये बात करती हैं। हर मैसेज एक टॉपिक पर पब्लिश होता है। हर टॉपिक का एक पब्लिशर होता है और एक या अधिक 
सब्सक्राईबर।
