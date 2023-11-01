FROM centos:7    
RUN yum install epel-release -y 
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/*
#RUN echo "Hello World" > /usr/share/nginx/html/index.html
COPY index.html /usr/share/nginx/html/index.html
#CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80
LABEL COMPONENT=nginx
ENTRYPOINT [ "nginx", "-g", "daemon off;" ]

### entry point
## CMD VS Entrypoint
# CMD is just a argument we can overide it
# entry point is not the actual command . when we donot want any one to overide the
## annyting we use entry point