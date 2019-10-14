# osrs-quest-api ![npm](https://img.shields.io/npm/v/osrs-quest-api.svg) [![Build Status](https://travis-ci.org/cerniglj1/osrs-quest-api.svg?branch=master)](https://travis-ci.org/cerniglj1/osrs-quest-api)

An api using json data to see if your account is able to complete certain quests. Uses the osrs-api package as well.



## Installation 
```
$ npm install --save osrs-quest-api
```

## Usage

### Get individual quest requirements
#### `has_levels_for_quest(quest_name)`
Used to get individual quest requirements


##### Example
```python
from quest_checker import QuestChecker
qc = QuestChecker('jimbo jango', 300)
qc.has_levels_for_quest('Regicide')
```

##### Output

<span style="color:blue">Regicide</span>

#### Get all quests that are can be done at the current levels of the account
#### `get_doable_quests()`

##### Example
```python
from quest_checker import QuestChecker
qc = QuestChecker('jimbo jango', 300)
qc.get_doable_quests()
```
