

### ubuntu 에서
sudo apt update  
sudo apt install mysql-server  

mysql_secure_installation

sudo mysql -u root -p 접속 

##### 안될시 auth_socket 인증모드사용중임
##### 따라서 native_password 모드로 변경

ALTER user'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';


API 에 DATABASE 연결

미리 테이블구조와 관계를 구현해놓아야함. SCHEMA 

 ## users
 id  
 name  
 email  
 profile  
 hashed_password  
 
 
 ## tweets
 id  
 user_id  
 tweet  
 
 ## user_follow_list
 id  
 user_id
 follow_user_id


