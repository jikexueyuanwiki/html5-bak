# Manifest 文件

manifest 文件是简单的文本文件，它告知浏览器被缓存的内容（以及不缓存的内容）。

manifest 文件可分为三个部分：

CACHE MANIFEST - 在此标题下列出的文件将在首次下载后进行缓存

NETWORK - 在此标题下列出的文件需要与服务器的连接，且不会被缓存

FALLBACK - 在此标题下列出的文件规定当页面无法访问时的回退页面（比如 404 页面）

**CACHE MANIFEST**

第一行，CACHE MANIFEST，是必需的：

```javascript
CACHE MANIFEST
/theme.css
/logo.gif
/main.js
```

上面的 manifest 文件列出了三个资源：一个 CSS 文件，一个 JS文件，以及一个 HTML 文件。当 manifest 文件加载后，浏览器会从网站的根目录下载这三个文件。然后，无论用户何时与因特网断开连接，这些资源依然是可用的。

**NETWORK**

下面的 NETWORK 小节规定文件 "login.asp" 永远不会被缓存，且离线时是不可用的：

```javascript
NETWORK:
login.asp
```

可以使用星号来指示所有其他资源/文件都需要因特网连接：

```javascript
NETWORK:
*
```

**FALLBACK**
下面的 FALLBACK 小节规定如果无法建立因特网连接，则用 "offline.html" 替代 /html5/ 目录中的所有文件：

```javascript
FALLBACK:
/html5/ /404.html
```

> 注：第一个 URI 是资源，第二个是替补。