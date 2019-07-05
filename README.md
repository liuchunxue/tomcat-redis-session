# tomcat-redis-session
支持tomcat8.5做session共享。 
tomcat  context.xml文件增加配置   这里有一个坑，password必须设置，不然会出问题
<Valve className="com.orangefunction.tomcat.redissessions.RedisSessionHandlerValve" /> 
	<Manager className="com.orangefunction.tomcat.redissessions.RedisSessionManager"
	host="127.0.0.1" 
	port="6379" 
	database="0" 
	password="123456" 
	maxInactiveInterval="60" />
