JasperReports-plugin
=============

This maven compiles Jasper files to the target directory.

Motivation
----------
The original jasperreports-maven-plugin from org.codehaus.mojo was a bit slow. This plugin is 10x faster. I tested it with 52 reports which took 48 seconds with the original plugin and only 4.7 seconds with this plugin.

Usage
-----
You can use the plugin by adding it to the plug-in section in your pom;

As Kanye West said:

> We're living the future so  
> the present is our past.

I think you should use an  
`<addr>` element here instead.

code:
```app/templates/scientists.hbs
# usage
<h2>List of Scientists</h2>
<h1>List of Scientists</h1>
```

code:
```html
<h2>List of Scientists</h2>
<h1>List of Scientists</h1>
```

code:

    # usage
    <h2>List of Scientists</h2>
    <h1>List of Scientists</h1>

code:

    <h2>List of Scientists</h2>

code:

    function fancyAlert(arg) {
      if(arg) {
        $.facebox({div:'#foo'})
      }
    }

<h1>Jasper options to the compiler</h1>

If you want to pass any Jasper options to the compiler you can do so by adding them to the configuration like so:

```xml
<plugin>
	...
	<configuration>
		...
		<additionalProperties>
			<net.sf.jasperreports.awt.ignore.missing.font>true</net.sf.jasperreports.awt.ignore.missing.font>
			<net.sf.jasperreports.default.pdf.font.name>Courier</net.sf.jasperreports.default.pdf.font.name>
			<net.sf.jasperreports.default.pdf.encoding>UTF-8</net.sf.jasperreports.default.pdf.encoding>
			<net.sf.jasperreports.default.pdf.embedded>true</net.sf.jasperreports.default.pdf.embedded>
           </additionalProperties>
	</configuration>
</plugin>
```

You can also add extra elements to the classpath using

```xml
<plugin>
	...
	<configuration>
		...
		<classpathElements>
			<element>your.classpath.element</element>
        </classpathElements>
	</configuration>
</plugin>
```
