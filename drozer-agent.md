# This tutorial for install `drozer-agent.apk` into your android genymotion

* **Download Drozer-Agent**

  Link [drozer-agent-2.3.4.apk](http://cdn-file.progress28.com/uploads/drozer-agent-2.3.4.apk)
  
  or download using `wget` command
  
  ```wget http://cdn-file.progress28.com/uploads/drozer-agent-2.3.4.apk```
  
  
* **Install into android genymotion using adb (first connect into your device before install apk)**
  
  ```adb install drozer-agent-2.3.4.apk```
  
  * **MacOS**
  
    ```
    macos@rootbakar ~ % adb install drozer-agent-2.3.4.apk                                
    Performing Push Install
    drozer-agent-2.3.4.apk: 1 file pushed, 0 skipped. 128.2 MB/s (633111 bytes in 0.005s)
	  pkg: /data/local/tmp/drozer-agent-2.3.4.apk
    Success
    ```
    
  * **Ubuntu**
    ```
    root@ubuntu-server:~# adb install drozer-agent-2.3.4.apk 
    drozer-agent-2.3.4.apk: 1 file pushed. 0.2 MB/s (633111 bytes in 2.551s)
	  pkg: /data/local/tmp/drozer-agent-2.3.4.apk
    Success
    ```
    
* **After `drozer-agent` success installed, now you must running `drozer-agent` via android genymotion**
    
    * **Before running**
    
      <img src=http://cdn-file.progress28.com/uploads/file-202008011596265336.png width=300px hight=1000px />
    
    * **After Running**
    
      <img src=http://cdn-file.progress28.com/uploads/file-202008011596265425.png width=300px hight=1000px />
      
* **Now connect your machine with `drozer-agent`**
    
    * **MacOS**
    
      Under Maintenance for installing drozer
      
    * **Ubuntu**
    
      Connect `adb` with `drozer-agent` using `adb forward`
    
      ```root@ubuntu-server:~# adb forward tcp:31415 tcp:31415```
      
      open `drozer console`
      
      ```
        root@ubuntu-server:~# drozer console connect
        Selecting 8a515cdcfeac860b (unknown ANDROID_PENTEST 6.0)

                    ..                    ..:.
                   ..o..                  .r..
                    ..a..  . ....... .  ..nd
                      ro..idsnemesisand..pr
                      .otectorandroidsneme.
                   .,sisandprotectorandroids+.
                 ..nemesisandprotectorandroidsn:.
                .emesisandprotectorandroidsnemes..
              ..isandp,..,rotectorandro,..,idsnem.
              .isisandp..rotectorandroid..snemisis.
              ,andprotectorandroidsnemisisandprotec.
             .torandroidsnemesisandprotectorandroid.
             .snemisisandprotectorandroidsnemesisan:
             .dprotectorandroidsnemesisandprotector.

        drozer Console (v2.4.4)
        dz> 
      ```
