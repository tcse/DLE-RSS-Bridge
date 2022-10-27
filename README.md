# DLE-RSS-Bridge
Интеграция проекта RSS-Bridge в структуру модулей для DataLife Engine

**Установка:**

Открыть корневой файл
.htaccess

найти в нем

	RewriteEngine On


и добавить ниже

	# rss-bridge  
	RewriteRule ^rss-bridge/index.php$ /engine/modules/mod_tcse/rss-bridge/index.php [L]
	RewriteRule ^rss-bridge/$ /engine/modules/mod_tcse/rss-bridge/index.php [L]
	RewriteRule ^rss-bridge/static/style.css$ /engine/modules/mod_tcse/rss-bridge/static/style.css [L]
	RewriteRule ^rss-bridge/static/HtmlFormat.css$ /engine/modules/mod_tcse/rss-bridge/static/HtmlFormat.css [L]
	RewriteRule ^rss-bridge/static/search.js$ /engine/modules/mod_tcse/rss-bridge/static/search.js [L]
	RewriteRule ^rss-bridge/static/select.js$ /engine/modules/mod_tcse/rss-bridge/static/select.js [L]
	RewriteRule ^rss-bridge/static/logo_600px.png$ /engine/modules/mod_tcse/rss-bridge/static/logo_600px.png [L]


Доступ к админке сервиса по ссылке
/rss-bridge/
