FROM centos:7    
RUN yum install epel-release -y 
RUN yum install nginx -y
# systemctl start nginx -y can be run here so we use CMD (raw commands)
CMD ["nginx", "-g", "daemon off;"]       
EXPOSE 80
ENV PROJECT=roboshop
ADD sample.txt /opt

#RUN useadd roboshop
#USER roboshop
#WORKDIR /home/roboshop
#