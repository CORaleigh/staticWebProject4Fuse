Create and serve up a static html via fuse

In Eclipse:
Create new Dynamic Web Project and check the box to generate web.xml

then add this to the web.xml

    <servlet-mapping>
		<servlet-name>default</servlet-name>
		<url-pattern>/apidocs/*</url-pattern>
	</servlet-mapping>
</web-app>

In the WebContent folder, create a subfolder called apidocs and create an index.html file in there.

Be sure that this subfolder name matches the url-pattern above

Installation:
osgi:install war:file:/Users/foleyc/Downloads/empImages.war?Web-ContextPath=edirectory

