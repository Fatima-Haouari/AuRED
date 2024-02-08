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
  "id": "AuRED_089",
  "rumor": "وباء كورونا وصل الى الامارات 75 إصابة في ابوظبي و 63 إصابة في دبي  تحذير للامتناع عن السفر الى الامارات حفاظًا على السلامه و عدم نقل الوباء . اللهم أحفظ المسلمين في كل مكان..." ,
  "label": "REFUTES"
  "timeline": [["https://twitter.com/WHOEMRO", "1223614769195900928", "س. هل استلام رسائل أو طرود من الصين مأمون؟\nج. نعم مأمون. الناس الذين يتلقون رسائل وطرود من الصين ليسوا معرضين لخطر الإصابة #بفيروس_كورونا المستجد. التحليلات السابقة تؤكد أن الفيروس لا يبقى حياً لفترة طويلة فوق أسطح الأشياء مثل الرسائل والطرود.  #2019nCoV https://t.co/8NkvDO77vO"],
   ["https://twitter.com/WHOEMRO", "1223608938136047616", "س. هل تحمي اللقاحات المضادة للالتهاب الرئوي من #فيروس_كورونا المستجد؟ج. لا. لقاحات الالتهاب الرئوي لا تحمي من فيروس كورونا المستجد. هذا الفيروس جديد ومختلف ويحتاج لقاحاً خاصاً به. الباحثون يعملون على تطوير لقاح مضاد لهذا الفيروس. #اعرف_الحقائق https://t.co/QTGmI2flo9"],
   ["https://twitter.com/mohapuae", "1223361274618183681", "تعرف على أعراض فيروس كورونا الجديد #فيروس_كورونا_الجديد #فيروس_كورونا#كورونا#وزارة_الصحة_ووقاية_المجتمع_الإمارات https://t.co/jWALFtA68m"],
   ["https://twitter.com/mohapuae", "1223279618372882432", "مقتطفات من مشاركة وزارة الصحة ووقاية المجتمع في معرض ومؤتمر الصحة العربي2020 من خلال مجموعة من مبادرات ومشاريع الرعاية الصحية المبتكرة تحت شعار "صحة الإمارات مسؤولية مشتركة"#وزارة_الصحة_ووقاية_المجتمع_الإمارات#معرض_ومؤتمر_الصحة_العربي_2020#صحة_الإمارات https://t.co/c69pHj6ffd"],
   ......],
  "evidence": [["https://twitter.com/WHOEMRO","1222506828694794240","أكدت اليوم @WHO ظهور أولى حالات فيروس كورونا المستجد في إقليم شرق المتوسط، بالإمارات العربية المتحدة. عقب تأكيد @mohapuae في 29 يناير.
كان 4 أفراد من نفس العائلة من مدينة ووهان الصينية وصلوا إلى الإمارات في بداية يناير 2020، وتم إدخالهم المستشفى بعد تأكد إصابتهم ب #فيروس_كورونا."]
,....]
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
