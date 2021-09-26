### directory tree 구조

```powershell
basicSetting
|   app.js
|   package-lock.json
|   package.json
|   webpack.config.js
|   
+---bin
|       www
|       
+---dist
+---public
|   |   index.html
|   |   
|   +---images
|   +---javascripts
|   \---stylesheets
|           style.css
|           
\---routes
        index.js
```



### 작업 순서



1. 

```shell
cd basicStting
npm install
```

2. basicSetting 폴더 이름 변경

3. 변경된 폴더 아래의 bin/www 파일에서

   ```js
   var debug = require('debug')('${변경된 폴더 이름 소문자}:server');
   ```

   으로 변경

4. package.json, package-lock.json 파일에서

   ```json
   {
       "name": "${변경된 폴더 이름 소문자}",
       ...
   }
   ```

   로 변경
