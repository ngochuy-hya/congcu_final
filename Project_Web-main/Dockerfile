# Sử dụng Tomcat chính thức + JDK 21
FROM tomcat:9.0.104-jdk21

# Xoá ứng dụng mặc định của Tomcat (tùy chọn)
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy file WAR của bạn vào Tomcat, đặt tên là ROOT.war để chạy ở /
COPY *.war /usr/local/tomcat/webapps/ROOT.war

# Mở port 8080
EXPOSE 8080

# Không cần ENTRYPOINT vì Tomcat sẽ tự start khi container khởi động