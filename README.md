# tech-memo
---

This repository is my tech notes.

## markdown
### Link
```
[Text](URL)
```

### Insert Image
```
![Alt Text](IMG_URL)
```

### Table
```
| TH(align Left) | TH(align center) | TH(align right) |
|:---|:---:|---:|
| Table Data | Table Data | Table Data |
```

example
| TH(align Left) | TH(align center) | TH(align right) |
|:---|:---:|---:|
| Table Data | Table Data | Table Data |


### PlantUML
~~~
```uml
A -> B: text A2B
B -> A: text B2A

A -> C: text A2C

class ClassA{
  String str
  void method()
}

class ClassB{
  Integer int
}

ClassA <|-- ClassB

```
~~~

example
```uml
A -> B: text A2B
B -> A: text B2A

A -> C: text A2C

class ClassA{
  String str
  void method()
}

class ClassB{
  Integer int
}

ClassA <|-- ClassB
```

## Links
|link|description|
|----|----|
| [Google App Scrips](/google/gas.md) | GAS全般 |