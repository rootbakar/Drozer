# Using `help` command for detail information #
    
```help scanner.provider.finduri```
</br>
</br>
```help app.provider.insert```
</br></br></br>
* **Running `app.activity.info` for view all activity information about some package**

    ```    
    dz> run app.activity.info -a jakhar.aseem.diva
    Package: jakhar.aseem.diva
      jakhar.aseem.diva.MainActivity
        Permission: null
      jakhar.aseem.diva.APICredsActivity
        Permission: null
      jakhar.aseem.diva.APICreds2Activity
        Permission: null
    ```    

* **Running `app.activity.start` for launch private activity from some package**

    ```
    dz> run app.activity.start --component jakhar.aseem.diva jakhar.aseem.diva.APICredsActivity
    ```
