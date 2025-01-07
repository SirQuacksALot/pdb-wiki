### Git - Version workflow
---

[ [Wiki](../../README.md) ] [ [Development](README.md) ]

---

> ### Desciption 📄
Here, we will describe how newly developed features will be added to the project through the version control git. The idea is to establish an overview of the workflow within the project and also give easy automation control with git actions.

> ### Branch structure 🌲
The branches are categorised branches, which means that they are named by a category. These are stable, dev, and exp. These branches are named as such and occur only once.

The exp branches are special in that they are named `exp_implementation_short_description` and can occur multiple times with different names. They should be used for step-by-step implementation of features and quick fixes.

> ### Releases 
Releases are a representation of the state of the project. They are created automatically by a git action workflow on branch creation, changes and merges. To clarify the different version types the release name will be in a specific format described as follows:

> Version Name Format: ` s.d.e `  
> `s` = stable version ➔  a set of features which are implemented are fully tested  
> `d` = development version ➔  new features are implemented and in testing  
> `e` = experimental version ➔  implementation of a new feature for debugging and testing  

Releases will be created as specified by the created experimental branch, the merge of an experimental branch into the dev branch and the merge from the dev to the stable branch. Depending on the last release version name and the way of creation (experimental creation, development merge or stable merge) the name of the new release will increase the respective digit. 

> ### Version Types (*Tags*) 📦
The version types are representative Tags for the releases. Those are three different category types which are **experimental**, **development** and **stable** and they go hand in hand with the branch structure.

The first version type will be **experimental**. In the numeric version name, it is displayed by the third number (v0.0.X) and is for highly unstable code which isn't tested yet. Its purpose is mostly debugging and testing like quick fixes or step-by-step implementation.

The second tag is **development** and it is displayed by the second number in the numeric display way (v0.X.0). It is for testing implemented features in a development environment. The dev branch's purpose is to serve a service which automatically syncs or installs the repo/program and gives the developer (a group of testers) the possibility to test and or debug the current state of the feature which is getting implemented into the state of the program.  

The third and last is the **stable**. Its numeric representation is the first number (vX.0.0). This branch is for the implementation of a stable feature or a set of tested and stable features. It is a representation of the production state of the service or program.  

```Examples: 1.6.372, 1.8.0, 2.0.0 ```
