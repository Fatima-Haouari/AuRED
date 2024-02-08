# Authority Rumor EviDence Dataset (AuRED)

## Content of this repository
## Rumors

We provide AuRED and AuRED* data in JSON format fileS. Each file contains a list of JSON objects representing rumors. For each rumor, we provide the following entries:
```
{
  id [unique ID for the rumor]
  rumor [rumor tweet text]
  label [the veracity label of the rumor eithr SUPPORTS, REFUTES, NOT ENOUGH INFO]
  timeline [authorities timeline associated with the rumor each authority tweet is represented by authority Twitter account link, authority tweet ID, authority tweet text]
  evidence [authorities evidence tweets represented by authority Twitter account link, authority tweet ID, authority tweet text]
}
```
Examples:

```
{
  "id": "AuRED_",
  "rumor": "وباء كورونا وصل الى الامارات 75 إصابة في ابوظبي و 63 إصابة في دبي  تحذير للامتناع عن السفر الى الامارات حفاظًا على السلامه و عدم نقل الوباء . اللهم أحفظ المسلمين في كل مكان..." ,
  "label": "REFUTES"
  "timeline": [["https://twitter.com/NCEMAUAE", "1222222840474238983", "RT @admediaoffice:ستشهد المنطقة المحيطة بمحطات براكة للطاقة النووية، والشاطئ الغربي من منطقة براكة في منطقة الظفرة صباح يوم غد، 29 يناير 2020، اختبارًا لصافرات الإنذار، والتي قد ينتج عنها أصوات عالية نسبياً قد يسمعها سكان المناطق المحيطة بالمحطات من الساعة 11:30 حتى 11:40 صباحاً."],[],[],......],
  "evidence": [[],[]]
},
...,
{
  "id": "AuRED_",
  "rumor": "" ,
  "label": "SUPPORTS",
  "timeline": [[],[],[],......],
  "evidence": [[],[]]
},
...
{
  "id": "AuRED_",
  "rumor": "" ,
  "label": "NOT ENOUGH INFO",
  "timeline": [[],[],[],......],
  "evidence": []
},

...

```
## Rumors folds
We provide the rumors 5 folds used in our experiments. Each fold file containing 32 rumors.
