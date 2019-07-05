# tomcat-redis-session
1、支持tomcat8.5
2.tomcat配置
	<Valve className="com.orangefunction.tomcat.redissessions.RedisSessionHandlerValve" />
	<Manager className="com.orangefunction.tomcat.redissessions.RedisSessionManager"
	host="127.0.0.1"
	port="6379"
	database="0"
	password="123456"
	maxInactiveInterval="60" />

	redis密码一定要设置，不能为空，不然有坑