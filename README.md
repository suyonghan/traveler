![screenShot_traveler](https://user-images.githubusercontent.com/35483497/61838216-399da800-aec3-11e9-8e08-1a238c5c14e6.jpg)
==========

## index
1. Getting started
    * Oracle Database 11g Express Edition
    * Spring framework
    * Config File
    * OpenWeatherMap
2. Tutorial
   * Authentication
      * singin
      * signup
      * find id/passwd
      * edit account info
   * Main
      * main_page
      * Chat
      * Weather & Position
   * Post
      * create post
      * display post

3. Error report
    * 403 error
  
 
### 1. Getting Started
1. Oracle Database 11g Express Edition
    ![screenshot database-diagram](https://user-images.githubusercontent.com/35483497/61840536-6efac380-aecc-11e9-9729-b0db10f4770e.PNG)
2. Spring frame work
   servlet.context
   ```
   <beans:bean id="dataSource"   //DB 계정 및 패스워드 설정
		class="org.springframework.jdbc.datasource.DriverManagerDataSource">
		<beans:property name="driverClassName"
			value="oracle.jdbc.OracleDriver" />
		<beans:property name="url"
			value="jdbc:oracle:thin:@localhost:1521:XE" />
		<beans:property name="username" value="USERNAME" />
		<beans:property name="password" value="PASSWORD" />
	</beans:bean>
   
   <websocket:handlers>   //웹소켓 매핑명 지정
		<websocket:mapping path="/chat"
			handler="myHandler" />
	</websocket:handlers>
   ```
3. Config File
   설정파일에서는 Database정보와 서버
   ```
   #### Oracle DB Info ####
   db.driver=oracle.jdbc.driver.OracleDriver
   db.url=jdbc:oracle:thin:@localhost:1521:orcl
   db.username=USERNAME
   db.password=PASSWORD

   #### File Path ####
   path.image=http://SERVER IP ADDRESS/traveler/resources/images
   #### Server IP Address Info ####
   ip.address=IPADDRESS
   ip.portNo=PORT#

   #### openWeather App Key info ####
   OpenWeather.appkey=APPKEY
   ```
4. OpenWeatherMap

### 2. Config File

### 3. tutorial
1. Authentication
   * signin
      ![screenshot_signin](https://user-images.githubusercontent.com/35483497/61838479-77e79700-aec4-11e9-8c79-913db154cae4.png)

   * signup
      ![screenshot_signup](https://user-images.githubusercontent.com/35483497/61838537-c1d07d00-aec4-11e9-9e34-42494df127a5.png)

   * find id/passwd
      ![screenshot_findId&passwd](https://user-images.githubusercontent.com/35483497/61838609-0d832680-aec5-11e9-8778-92d71a076344.PNG)
      
      
   * edit account info
      ![screenshot_mypage1](https://user-images.githubusercontent.com/35483497/61838660-48855a00-aec5-11e9-9721-8c8902d52c6d.PNG)
      ![screenshot_mypage2](https://user-images.githubusercontent.com/35483497/61838662-49b68700-aec5-11e9-8cb3-3551c68b2ff4.PNG)
2. Main
   * main page
   ![screenshot_main1](https://user-images.githubusercontent.com/35483497/61839481-abc4bb80-aec8-11e9-99d1-c52a2554c940.PNG)
   ![screenshot_main2](https://user-images.githubusercontent.com/35483497/61839482-abc4bb80-aec8-11e9-9c9e-c86b6bad0631.PNG)
   * chat
      ![screenshot_chat](https://user-images.githubusercontent.com/35483497/61839485-abc4bb80-aec8-11e9-89d3-babfcc1606c5.png)
   * weather & Map
      ![screenshot_weather&map](https://user-images.githubusercontent.com/35483497/61839484-abc4bb80-aec8-11e9-8706-4d72f20c55ab.PNG)
3. Post
   * create post
   ![screenshot_post1](https://user-images.githubusercontent.com/35483497/61839424-6b653d80-aec8-11e9-8005-2eae356715a7.PNG)
   * display post
   ![screenshot_post2](https://user-images.githubusercontent.com/35483497/61839422-6acca700-aec8-11e9-9eb8-933804f4219a.PNG)

### 3. Error report
   1. 403 error
   ![error403](https://user-images.githubusercontent.com/35483497/61839778-d5caad80-aec9-11e9-8873-748858dddcee.PNG)

