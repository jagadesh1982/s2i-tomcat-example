# s2i-tomcat-example
s2i-tomcat-example


Basic Example for creating a S2i Model

create .s2i directory
create bin in the .s2i
create assemble , run and usage files in the bin location

assemble - used in building the image
run - will be used as a entry point for running the image

Build the Docker image using - docker build -t s2i-tomcat .
Build the application Source Image using s2i - s2i build /root/myApp/ s2i-tomcat s2i-tomcat-app --loglevel=5 &> /tmp/s2i.log



Make sure you have a /root/myApp directory where your war file exists for copying into the tomcat in the container.
