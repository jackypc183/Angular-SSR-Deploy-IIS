ng build --base-href /ssr/

然後要把build後從browser資料夾裡面把server.js、web.config移出來跟browser同一層


 Run SSR App

    - powershell

    - ```powershell

    $env:PORT = "1234"  # listen port

    $env:RelativePath = "/test1" # website subfolder ex.[www.ooxx.com/test1/](https://www.ooxx.com/test1/ "https://www.ooxx.com/test1/")

    node.exe server.js

    ```

    - IIS

    - Web.config

    -   ```xml

    `<appSettings>`

    `<add key="PORT" value="1234" />` `<!-- listen port -->`

    `<add key="RelativePath" value="/test1" />` `<!-- website subfolder ex. [www.ooxx.com/test1/-->`](https://www.ooxx.com/test1/--> "https://www.ooxx.com/test1/--%3e")

    `</appSettings>`

    ```
