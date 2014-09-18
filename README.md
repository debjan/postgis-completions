##Instructions##


### Sublime Text ###

Copy `PostGIS.sublime-completions` to User packages

![](http://i.imgur.com/xsSLeRg.png)


### SciTE ###

Copy `PostGIS.api` to `api` subfolder relative to `SciTE.exe` location

Append this block to `sql.properties` file:

	file.patterns.pgsql=*.pgsql
	lexer.$(file.patterns.pgsql)=sql
    
    calltip.sql.word.characters=_$(chars.alpha)$(chars.numeric)
    calltip.sql.end.definition= 
    calltip.sql.parameters.start=(
    calltip.sql.parameters.end=)
    calltip.sql.parameters.separators=,
    calltip.sql.use.escapes=1
    autocomplete.sql.ignorecase=1

	api.$(file.patterns.sql)=$(SciteDefaultHome)/api/postgis.api
	api.$(file.patterns.pgsql)=$(SciteDefaultHome)/api/postgis.api

![](http://i.imgur.com/QW9XLy5.png)

![](http://i.imgur.com/Uu67R6q.png)