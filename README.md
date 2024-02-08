# AuRED
Authority Rumor EviDence Dataset (AuRED)

## Content of this repository
## Rumors

We provide the rumors in a JSON format file. The file contains a list of JSON objects representing rumors. For each rumor, we provide the following entries:
```
{
  id [unique ID for the rumor]
  claim [rumor tweet text]
  label [the veracity label of the rumor eithr SUPPORTS, REFUTES, NOT ENOUGH INFO]
  timeline [authorities timeline associated with the rumor each authority tweet is represented by authority Twitter account link, authority tweet ID, authority tweet text]
  evidence [authorities evidence tweets represented by authority Twitter account link, authority tweet ID, authority tweet text]
}
```
Examples:

```
{
  "id": "AuRED_",
  "claim": ,
  "label": "REFUTES"
  "timeline": ,
  "evidence": 
},
...,
{
  "id": "AuRED_",
  "claim": "" ,
  "label": "SUPPORTS",
  "timeline": "بعد تعينه نائب رئيس الجمعية الدستورية القطرية الرئيس قيس سعيد يقسم اليمين امام صاحبة السمو الشيخة موزة المسند فى عاصمة #قطر الدوحة https://t.co/kCYFDQHYcS",
  "evidence": "politics"
},
...

```
## Rumors folds
We provide the rumors 5 folds used in our experiments. Each fold file containing 32 rumors.
