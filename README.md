# README

This is the anonymized repository of  **AutoLog.**

![1663063757857](image/README/1663063757857.png)

The repository consists of multiple folders. The folder `/src` includes source code. The folder `/data` contains the generated demo data from AutoLog. The folder `/scripts` contain some useful scripts. The folder `/third-party` includes two open-source program analysis tools we adpated in this project. The folder `/build` contains some builded artifacts.

### Generated Datasets

The demo datasets are shown in the data folder.

**Sample:**

```json
{"9E4C996176B68B9A5F521819A453BB91": {"templates": [......, 
"Resolved path is  <*> ",
 "ACCESS CHECK:  this , doCheckOwner= <*> , ancestorAccess= <*> , parentAccess= <*> , access= <*> , subAccess= <*> , ignoreEmptyDir= <*> , resolveLink= <*> ",
"UnresolvedPathException  path:  <*>  preceding:  <*> count:  <*>  link:  <*>  target:  <*>  remainder:  <*> ",
"Could not get full path. Corresponding file might have deleted already.",
"Could not get full path. Corresponding file might have deleted already."
], "label": 1}
```

For more data, you can get it from: [AutoLogData](https://drive.google.com/drive/folders/197rHozOtNgM6ZzSVLKJ2Kd9sXvAlb3Uo?usp=sharing) & [Pupolar50](https://github.com/ICSE2023AutoLog/ICSE2023AutoLog/tree/main/data)

### Execution

You can play with this analysis framework with multiple ways.

* `LogStatGen.jar`: fetch and restore log statements from analyzed artifacts for preliminary labelling.
* `LogEPGen.jar`: acquire log-related execution paths.
* `javacg.jar`: generate call graph from java project.
* `log_methods_generator.py`: a simple way to generate pruned call graphs.
* `AutoLog_generator.py`: log path walking.
