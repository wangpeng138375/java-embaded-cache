下载jar包导入 项目，并在web.xml中添加如下配置即可使用
> <!-- 指定缓存清理周期，系统将在指定时间间隔后对缓存进行清理  若不设定则默认为10分钟-->
> 

&lt;context-param&gt;


> > 

&lt;param-name&gt;

period

&lt;/param-name&gt;


> > 

&lt;param-value&gt;

60000

&lt;/param-value&gt;



> 

&lt;/context-param&gt;


> <!-- 指定缓存中值存在的时间，值将过期被清理程序清理  若不设定该值默认为半小时-->
> 

&lt;context-param&gt;


> > 

&lt;param-name&gt;

expires

&lt;/param-name&gt;


> > 

&lt;param-value&gt;

180000

&lt;/param-value&gt;



> 

&lt;/context-param&gt;


> 

&lt;listener&gt;


> > 

&lt;listener-class&gt;

com.yong.cache.WebCacheListener

&lt;/listener-class&gt;



> 

&lt;/listener&gt;

