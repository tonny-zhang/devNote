#How to debug phonegap Application with weinre!
   

1.install weinre.
    ```
      $ npm -g install weinre
    ```
`
    Notice: You should install nodejs and npm first.
   
2.start weinre
    $ weinre --boundHost __IP_address__ --httpPort __port__

> Notice: Then weire will startup at special ip address what you typed.
> You should type in a effective ip. If you use localhost or 127.0.0.1, then you can't debug application in you device.
> You can type an ip like 192.168.1.100, so you can debug your app in your device with this IP.

   
3.open browser
    Open your chrome, goto http://__IP_address__:__port__.
  
    Notice: You can change the ip address and the httpPort. It's defined by you when start weinre.

   
4.add script to App
    Add script to your own app. Just like this:
    `<script src="http://192.168.1.100:8080/target/target-script-min.js#anonymous"></script>`
  
    Notice: The ip address and port should same as your weinre settings. Also same as your browser address.

   
5.begin to debug.
    Now, you can debug your application as web pages in your browser.
