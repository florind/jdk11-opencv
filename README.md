# Docker image that combines OpenJDK 11 and OpenCV 4.0

The opencv-4.1.2.jar and the statically linked .so are installed in `/usr/local/share/java/opencv4`. 

# Example building a project
To build an openCV 4.0.x & JDK11 based project, use this command (gradle project):
`LD_LIBRARY_PATH=/usr/local/share/java/opencv4 ./gradlew -Djava.library.path=/usr/local/share/java/opencv4 build`

To run, use:
`LD_LIBRARY_PATH=/usr/local/share/java/opencv4 java -jar your-fatjar.jar`
