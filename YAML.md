## YAML

* This is data representation format, which uses name/value pairs
* It is collection of name value or key value pair used to represent data.
* Generally it is stored in files with extension .yml or .yaml

* The basic format is `<name>: <value>`
* `topic: Docker`

*  Values can be of different types / types of data

* Simple
     * text: can be represented in single or double quotes tool: ansible
     * number: numbers in non quote format `age: 10`
     * boolean: true, false, yes, no `online: yes`   
  
       * Simple/Scalar
           * Text
           * number
           * boolean

* Complex
     
     * list: array
       colors:
         – black
         – white
     
       * Complex
        
           * list/array
           * map/dictionary/object

* Extension of YAML files is `.yaml` or `.yml.` YAML is a text file
* Simple yaml 

```
url: directdevops.blog
author: khaja
isDailyUpdated: true
isLoginRequired: false
articlecount: 1000
```

* List example

```
---
Colors:
  - Black
  - White
Movies:
  - Avengers
  - Batman Begins

```

* Map/Dictionary/object

```
---
Address:
  flatno: 407
  building: Mythrivanam
  area: Ameerpet
  city: Hyderabad
```

* yaml about Quality Thought

```
---
name: QualityThought
url: https://qualitythought.in
courses:
  - name: Azure
    faculty: khaja
    duration: 90
  - name: AWS
    faculty: khaja
    duration: 90
  - name: DevOps
    faculty: khaja
    duration: 110
  - name: Manual Testing
    faculty: Ramana
    duration: 60
Branches:
  headoffice:
    flatno: 302
    building: nilgiri
    city: hyderabad
  devops:
    flatno: 407
    building: mythrivanam
    city: hyderabad
```

* We have list out names/keys then we need fill values
  
```
name = text
phone number = text
email text
professional summar text
skillset
   <skill name>: <skill values>
work experience: 
    experience list:
        company name
        duration
        role and responsibilities: text array/list

```


* Try writing about yourself in a yaml according to following structure

```
---
#qualification
yearofpassing: <number>
university: <text>
grade: text (A+|A|B|C)
----
# education
<name>: <qualification>

----
name: <text>
mobile: <text>
email: <text>
education: list(<education>)
```

* Example 1 (Postgraduate)

```
---
name: vishnu
mobile: '999999999'
email: vishnu@gmail.com
education:
  - mtech:
      yearofpassing: 2017
      university: jnu
      grade: A
  - btech:
      yearofpassing: 2015
      university: jntu
      grade: A+
```

* Example (graduate – BSc)

```
---
name: Swathi
mobile: '88888888'
email: swathi@outlook.com
education:
  - BSc:
      yearofpassing: 2020
      university: osmania
      grade: A+
```

* YAML will be used to define kuberentes manifests and docker compose files
* YAML documentation from ansible refer here: https://docs.ansible.com/ansible/latest/reference_appendices/YAMLSyntax.html