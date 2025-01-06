### Git - Version workflow
---

[ [Wiki](../../README.md) ] [ [Development](README.md) ]

---

> ### Desciption 📄
Here will be described how newly developed features will be added to the project throgh the version controll git. The idea is to establish a overview of the workflow within the projekt and also give easy automation controll with git actions.

> ### Branch structure 🌲
The branches are categiresed branches wich means that they are named by a categorie. These are stable, dev and exp. These branches are named as such and occure only once.

The exp branches a special in the way that they are named in the following way: `exp_implementation_short_description` and can occure multiple times with different names. They should be use for step by step implementation of features and quick fixes.

> ### Version Types (*Tags*) 📦
The version types are represented by Tags for the releases. Wich are created automaticly by a git action workflow. They are created on branch creation chnages and merges.

> Version Format: ` s.d.e `  
> `s` = stable version - a set of features wich are implemented are fully tested  
> `d` = development version - new features are implemented and in testing  
> `e` = experimental version - implementation of new feature for debugging and testing

The first version type will be **experimental**. In the numeric version name it is displayed by the third number (v0.0.X) an is for highly unstable code wich isnt tested yet. Its purpose is mostly debugging and testing like quick fixes or step my step implemtation.

The second is **development** and it is displayed by the second number in the numeric display way (v0.X.0). It is for testing a implemented features in a development enviornment. The dev branches purpose is to server a service wich automaticly syncs or installes the repo / programm and give the developer (a groupe of testers) the possibility to test and or debug the current state of the feature wich is getting implemented into the state of the programm.  

The third and last branch is the **stable** branch. Its numeric represetaion is the first number (vX.0.0). This branch is for the implementation of a stable feature or a set of tested and stable features. It is a representation of the production state of the service or programm.  

```Examples: 1.6.372, 1.8.0, 2.0.0 ```