## REF
- https://www.cnblogs.com/shineqiujuan/p/4703304.html
- https://blog.csdn.net/mydo/article/details/54377021
- https://www.cnblogs.com/LazyCout/p/7839000.html

## Environment
macOS High Sierra version 10.13.3

# INSTALL via HOMEBREW
1. 
<pre><code>brew install postgresql
</code></pre>

# START & STOP
Start:
<pre><code>pg_ctl -D /usr/local/var/postgres -l /usr/local/var/postgres/server.log start
</code></pre>

Stop:
<pre><code>pg_ctl -D /usr/local/var/postgres stop -s -m fast
</code></pre>

# CREATE USER
<pre><code>createuser username -P
</code></pre>
回车输入 2 次用户密码后即用户创建完成。

# CREATE & DROP DATABASE
### create a database
<pre><code>createdb database_name -O user_name -E UTF8 -e
</code></pre>
* database_name: 创建了一个名为 dbname 的数据库
* user_name: 指定 username 为改数据库的拥有者（owner）
* -E UTF8: 数据库的编码（encoding）是 UTF8
* -e: 把数据库执行操作的命令显示出来

 **Attention: it seems that '-' is not legal in a PostgreSQL identifier.**

### link(? lianjie) a database
<pre><code>psql -U user_name -d database_name
</code></pre>



<pre><code>
</code></pre>
<pre><code>
</code></pre>

# CREATE & DROP TABLE

# COMMON OPERATIONS
