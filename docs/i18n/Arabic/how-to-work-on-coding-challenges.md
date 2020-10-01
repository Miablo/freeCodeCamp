# كيفية العمل على تحديات البرمجة

هدفنا هو تطوير تجربة تعلم تفاعلية ممتعة وواضحة.

وتصميم تحديات البرمجة التفاعلية أمر صعب. سيكون من الأسهل بكثير كتابة شرح طويل أو إنشاء دروس فيديو، وهناك مكان للذين على موقع متوسط و يوتيوب. لكن، بالنسبة لمنهجنا الأساسي، نحن ملتزمون بما يصلح لمعظم الناس - تجربة تفاعلية تماما وشبه تجربة لعبة الفيديو.

نريد أن تحقق الكاميرات حالة التدفق. ونريد منهم أن يبنوا زخما وأن ينفجروا من خلال منهجنا الدراسي بأقل عدد ممكن من الزجاج. ونريد لهم أن يدخلوا في المشاريع بثقة وأن يتعرفوا على نطاق واسع على مفاهيم البرمجة.

ويتطلب خلق هذه التحديات إبداعا هائلا واهتماما بالتفاصيل. هناك الكثير من المساعدة المتاحة. ستحصل على دعم من فريق كامل من المساهمين الذين يمكنك أن ترتدي أفكارك وتجريب تحدياتك. ابقى نشطا في [غرفة المساهمين](https://gitter.im/freecodecamp/contributors) واطرح الكثير من الأسئلة.

بمساعدتك يمكننا تصميم منهج تعليمي تفاعلي سوف يساعد ملايين الناس على تعلم البرمجة لسنوات قادمة.

يتم تخزين محتوى كل تحدي في ملف markdown الخاص به. يتم تحويل هذا الملف في وقت لاحق إلى HTML باستخدام أدواتنا لإنشاء صفحات ويب تفاعلية.

يمكنك العثور على كل محتوى المنهج الدراسي لـ freeCodeCamp.org's في دليل [`/curriculum/challenges`](https://github.com/freeCodeCamp/freeCodeCamp/tree/master/curriculum/challenges).

## إعداد أدوات المنهج الدراسي

قبل أن تعمل على المناهج الدراسية، ستحتاج إلى إعداد بعض الأدوات لمساعدتك على اختبار التغييرات الخاصة بك. يمكنك استخدام أي خيار من الأسفل:

- يمكنك [إعداد FreCodeCamp محليا](how-to-setup-freecodecamp-locally.md). هذه **موصى بها بشدة** للمساهمات العادية/المتكررة. هذا الإعداد يسمح لك بالعمل واختبار التغييرات الخاصة بك.
- استخدام Gitpod، بيئة ديف مجانية على الإنترنت. النقر على الزر أدناه سيبدأ بيئة dev جاهزة للبرمجة الحرة في المتصفح الخاص بك. ويستغرق الأمر بضع دقائق فقط.

  [![فتح في Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/freeCodeCamp/freeCodeCamp)

- تعديل الملفات على واجهة GitHub، بالنقر على أيقونة قلم الرصاص للملف المقابل. في حين أن هذا هو أسرع طريقة، فإنه **غير مستحسن**، لأنك غير قادر على اختبار التغييرات الخاصة بك على GitHub. إذا خلص المشرفون لدينا إلى أن التغييرات التي أجريتها تحتاج إلى أن تختبر محلياً، سوف تحتاج إلى اتباع الأساليب أعلاه بدلاً من ذلك مرة أخرى.

## قالب التحدي

فيما يلي قالب لماهية التحديات التي تبدو عليها ملفات الدرجات السفلى حاليا.  لمشاهدة القالب المبسط سنعتمد [أنظر أدناه](#upcoming-challenge-template).

````md
---
المعرف: معرف فريد (أبجدي رقمي, MongoDB_id)
العنوان: عنوان التحدي
تحدي: 0
فيديوورل: 'رابط تفسير الفيديو'
---

## وصف

<section id='description'>
وصف للتحدي وما هو مطلوب لتمرير
</section>

## تعليمات

<section id='instructions'>
تعليمات حول ما يجب القيام به بالضبط.
</section>

## اختبارات

<section id='tests'>

```ml
اختبار:
  - نص: يجب أن يعيد "foo'
    اختبار String: 'دالة سلسلة ربما باستخدام تأكيد تشاي'
````

</section>

## بذرة التحدي

<section id='challengeSeed'>

<div id='{ext}-seed'>

```{ext}
الكود المعروض في المحرر بشكل افتراضي.

وهذا جزء مطلوب لهذا التحدي.
```

</div>

### قبل الاختبار

<div id='{ext}-setup'>

```{ext}
رمز اختبار اختياري.
```

</div>

### بعد الاختبار

<div id='{ext}-teardown'>

```{ext}
اختبار اختياري لتمزيق التعليمات البرمجية.
```

</div>

</section>

## حل

<section id='solution'>

```{ext}
// الحل مطلوب
```

</section>

````

> [!NOTE]
>
> 1. في الفروع الواردة أعلاه، أمثلة على `{ext}` هي:
>
>   - `html` - HTML/CSS
>   - `js` - JavaScript
>   - `jsx` - JSX
>
> 2. بالنسبة لقسم `الاختبارات` أعلاه، ينبغي أن تكون `text` و`testString` سلاسل YAML صالحة. 'testString' يمكن أن تكون دالة أو تعبير متسلسل يمكن أن تستخدم مزاعم تشاي.

## تحديات الترقيم

كل تحد يحتاج إلى `معرف`. إذا لم تحدد واحداً، سيقوم MongoDB بإنشاء واحد عشوائي جديد عندما يحفظ البيانات؛ ومع ذلك، نحن لا نريد أن نفعل ذلك، لأننا نريد أن تكون معارف التحدي متسقة عبر بيئات مختلفة (الإنتخابات التدريجية)، الإنتاج والكثير من المطورين المختلفين، إلخ.).

لإنشاء واحدة جديدة في قذيفة (بافتراض أن MongoDB يعمل بشكل منفصل):

1. تشغيل الأمر `mongo'.
2. تشغيل الأمر `objectId()'.

على سبيل المثال:

```bash
$ mongo
MongoDB Shell version v3.6.1
يتصل بـ: mongodb://127.0.0.1:27017
MongoDB Sersion: 3.4.10
...
$ ObjectId()
ObjectId("5a474d78df58bafeb3535d34")
````

النتيجة هي معد جديد، على سبيل المثال `5a474d78df58bafeb3535d34` أعلاه.

بمجرد أن يكون لديك بريدك، وضعه في ملف markdown كحقل `معرف` في الأعلى، على سبيل المثال.

```yml
---
المعرف: 5a474d78df58bafeb3535d34
عنوان: عنوان التحدي
```

## تحديات التسمية

تسمية الأشياء أمر صعب. لقد جعلنا الأمر أسهل من خلال فرض بعض القيود.

يجب أن تكون جميع عناوين التحدي صريحة ويجب أن تتبع هذا النمط:

\[verb\]\[شرط الكائن\]

فيما يلي بعض أسماء التحديات :

- استخدام التدوين على مدار الساعة لتحديد تعبئة العنصر
- مصفوفات مكثفة مع .خفض
- استخدم رمز مجموعة للعثور على الشخصية الأولى في سلسلة

## أوصاف/تعليمات التحدي

يجب أن تكون العقوبات واضحة وموجزة مع الحد الأدنى من الجرذون. وفي حالة استخدامها، ينبغي تعريف الجارجون فوراً باللغة الإنكليزية الواضحة.

إبقاء الفقرات قصيرة (نحو 1-4 جملة). ومن المرجح أن يقرأ الناس عدة فقرات قصيرة أكثر مما يقرأ جدارا للنص.

نص التحدي يجب أن يستخدم الشخص الثاني ("أنت") للمساعدة في إعطائه صوت محادثة. وبهذه الطريقة يبدو أن النص والتعليمات تتحدث مباشرة إلى كاميرا تعمل من خلال التحدي. حاول تجنب استخدام الشخص الأول ("I", "we", "let's", and "us").

لا تستخدم الروابط الصادرة. وهي تعرقل التدفق. وينبغي ألا يضطر كاميرون أبداً إلى إخفاء أي شيء خلال هذه التحديات. إذا كانت هناك موارد تعتقد أن كاميرات ستستفيد منها، فتضيفها إلى المقالة المتعلقة بالدليل الخاص بالطعن.

يمكنك إضافة رسوم بيانية إذا كان ذلك ضرورياً.

لا تستخدم الرموز التعبيرية أو الرموز التعبيرية في التحديات. FreCodeCamp لديه مجتمع عالمي، والمعنى الثقافي للرموز التعبيرية أو الانفعالية قد يكون مختلفا حول العالم. أيضًا، الرموز التعبيرية يمكن أن تكون مختلفة في أنظمة مختلفة.

الأسماء المناسبة يجب أن تستخدم الرسملة الصحيحة عندما يكون ذلك ممكنا. وترد أدناه قائمة بالكلمات التي ينبغي أن تظهر في التحديات.

- JavaScript (الأحرف الكبيرة في "J" و "S" و لا اختصار)
- Node.js
- تطوير الطرف الأمامي (شكل الصفة مع الشرطة) عندما تعمل على الطرف الأمامي (شكل اسم بدون شرطة). وينطبق نفس الشيء على "الطرف الخلفي" و"المكدس الكامل" والعديد من المصطلحات المركبة الأخرى.

### قاعدة دقيقتين

وينبغي أن يكون كل تحد قابلا للحل في غضون 120 ثانية بواسطة متحدث إنكليزي أصلي أكمل التحديات التي أدت إليه. هذا يشمل الوقت الذي يستغرقه قراءة الاتجاهات/التعليمات التي تفهم رمز البذر، اكتب التعليمات البرمجية الخاصة بهم واحصل على جميع الاختبارات لتمريرها.

إذا استغرق إكمال التحدي أكثر من دقيقتين، فلديك خياران:

- تبسيط التحدي، أو
- تقسيم التحدي إلى تحديين.

قاعدة دقيقتين تجبرك ، مصمم التحدي ، على جعل توجيهاتك موجزة، رمز البذور الخاص بك واضحة، واختبارك واضح.

نحن نتعقب الوقت الذي تستغرقه الكاميرات لحل التغييرات واستخدام هذه المعلومات لتحديد التحديات التي تحتاج إلى التبسيط أو التقسيم.

### الوحدة

وينبغي لكل تحد أن يدرس مفهوما واحدا بالضبط، وينبغي أن يكون هذا المفهوم واضحا من اسم التحدي.

يمكننا تعزيز المفاهيم التي سبق تغطيتها من خلال التكرار والتغييرات - على سبيل المثال، • إدخال عناصر h1 في تحد واحد، ثم عناصر h3 في وقت لاحق.

وهدفنا هو أن نواجه الآلاف من التحديات لمدة دقيقتين. ويمكن أن تتدفق هذه المفاهيم معا وتكرر تأكيد المفاهيم التي كانت مشمولة سابقا.

### تنسيق نص التحدي

وفيما يلي مبادئ توجيهية محددة بشأن التنسيق للنص الخاص بالتحدي والأمثلة:

- كلمات اللغة الرئيسية تدخل في `<code>` العلامات. على سبيل المثال، أسماء علامات HTML أو أسماء خصائص CSS
- المثيل الأول لكلمة مفتاحية عند تعريفها، أو الكلمات المفتاحية العامة (أي "الكائن" أو "الثابت") تذهب إلى `<dfn>` العلامات
- الإشارات إلى أجزاء التعليمات البرمجية (أي الدالة أو الطريقة أو أسماء المتغير) ينبغي تغليفها في `<code>` العلامات. انظر المثال أدناه:
- استخدم <code>parseInt</code> لتحويل المتغير <code>الواقع رقم</code> إلى عدد صحيح.
- يجب أن يسبق كتل التعليمات البرمجية متعددة الأسطر **سطر فارغ**. يجب أن يبدأ السطر التالي بثلاث خلفيات يعقبها مباشرة واحدة من [اللغات المدعومة](https://prismjs.com/#supported-languages). لإكمال كتلة التعليمات البرمجية، يجب عليك بدء سطر جديد يحتوي فقط على ثلاث خلفيات و **سطر فارغ آخر**. **ملاحظة:** إذا كنت ستستخدم رمز مثال في YAML ، استخدم `yaml` بدلاً من `yml` للغة إلى يمين الخلف.

انظر المثال أدناه:

````md
فيما يلي مثال على التعليمة البرمجية:

```{language}

[YOUR CODE HERE]

````
````

- ينبغي تنسيق معلومات إضافية في شكل ملاحظة `<strong>ملاحظة:</strong> استعرض نص الملاحظة...
- إذا كانت هناك حاجة إلى ملاحظات متعددة، ثم قم بقائمة جميع الملاحظات في جمل منفصلة باستخدام تنسيق `<strong>الملاحظات:</strong> نص الملاحظة الأولى. الحاشية الثانية نص.`.
- استخدام عبارات اقتباس مزدوجة حيث ينطبق

## اختبار الكتابة

يجب أن تحتوي التحديات على الحد الأدنى من الاختبارات اللازمة للتحقق من أن الكاميرا يفهم مفهوما.

وهدفنا هو الإبلاغ عن النقطة الوحيدة التي يحاول التحدي تعليمها، واختبار أنهم فهموا تلك النقطة.

يمكن أن تستخدم اختبارات التحدي مكتبات تأكيد Node.js و Chai.js. أيضًا، إذا لزم الأمر، يمكن الوصول إلى التعليمات البرمجية التي ينشئها المستخدم في متغير "الكود".

## تنسيق رمز البذور

إليك مبادئ توجيهية محددة لتنسيق رمز البذور التحدي:

- استخدم مسافتين لدخول
- بيانات جافا سكريبت تنتهي بفاصلة منها
- استخدم اقتباسات مزدوجة حيثما ينطبق
- التعليقات التي تم الإدلاء بها يجب أن يكون لها مساحة بين أحرف التعليق والتعليق نفسه

  `// اصلاح هذا السطر`

## تلميحات وحلول

لكل تحد زر 'احصل على تلميح`، حتى يتمكن المستخدم من الوصول إلى أي تلميحات/حلول تم إنشاؤها للتحدي. توجد مواضيع تلميح/حلول المناهج الدراسية في [منتدانا] (https://forum.freecodecamp.org/c/guide) تحت فئة `الدليل'.

إذا وجدت مشكلة مع موضوع تلميح/حلول التحدي القائم، يمكنك تقديم اقتراحات في [فئة المساهمين] (https://forum.freecodecamp.org/c/contributors) في المنتدى. وسيقوم المشرفون والمستعملون ذوو المستوى 3 باستعراض التعليقات ويقررون ما إذا كانوا سيدرجون التغييرات في موضوع التلميح/الحلول المقابل.

### إضافة تلميحات/مواضيع جديدة للتحدي

اتخاذ الخطوات التالية عند إضافة تلميحات/حلول جديدة للتحدي.

1. ابدأ باتباع نفس الخطوات لإنشاء موضوع جديد ولكن راجع التالي لإنشاء العنوان.
2. ينبغي أن يبدأ عنوان الموضوع بـ 'دليل تحدي FreCodeCamp Challenge: ' متوافق مع العنوان الفعلي لتحدي المنهج الدراسي. فعلى سبيل المثال، إذا كان التحدي يسمى "`قرود شونكي`"، فإن عنوان الموضوع سيكون "`دليل تحدي freeCodeCamp Guide: Chunky Monkey`".
3. يجب أن يكون "الكامبربوت" مالك هذه المواضيع/المشاركات، لذا ستحتاج إلى طلب مشرف لتغيير ملكية الوظيفة الرئيسية إلى 'الكاميربوت`.
4. بمجرد إنشاء الموضوع الجديد، يتم إنشاء معرف موضوع المنتدى. يقع في نهاية عنوان URL لموضوع المنتدى. يجب إضافة هذا المعرف إلى الموضوع الأمامي لملف تحدي المنهج الدراسي من خلال عملية طلب السحب العادية لزر "الحصول على تلميح" لربط الموضوع.

### مبادئ توجيهية لمحتوى التلميحات ومواضيع الحلول

عند اقتراح حل لموضوع الدليل المتصل بتحدي المنهج، يجب إضافة الرمز الكامل. وهذا يشمل جميع شفرة البذور الأصلية بالإضافة إلى أي تغييرات لازمة لتجاوز جميع اختبارات التحدي. يجب استخدام القالب التالي عند إنشاء تلميحات/مواضيع حلول:

``md
# اسم التحدي هنا

---

## شرح المشكلة

يلخص ما يجب القيام به دون مجرد تكرار وصف التحدي و/أو التعليمات. هذا قسم اختياري

#### الروابط ذات الصلة

- [Link Text](link_url_goes_here)
- [Link Text](link_url_goes_here)

---

## # # Hints

#### Hint 1

Hint هنا

#### 2

تلميح هنا

---

## # الحلول

<details><summary>الحل 1 (اضغط على عرض/Hide)</summary>

```js
function myFunc() {
  console. og('مرحبا بالعالم!');
}
````

#### شرح التعليمات البرمجية

- تفسير الرمز يذهب هنا
- تفسير الرمز يذهب هنا

#### الروابط ذات الصلة

- [نص الرابط](link_url_goes_here)
- [نص الرابط](link_url_goes_here)

</details>
````

## اختبار التحديات

أمامك [إنشاء طلب سحب] (كيف يمكن فتح - سحب الطلب). (د) بالنسبة للتغييرات الخاصة بك، تحتاج إلى التحقق من أن التغييرات التي قمت بها لا تسبب مشاكل مع التحدي عن غير قصد. 

1. لاختبار جميع التحديات تشغيل الأمر أدناه من الدليل الجذر

````
npm تشغيل الاختبار:منهج دراسي
``` 

2. يمكنك أيضا اختبار كتلة أو كتلة خارقة من التحديات باستخدام هذه الأوامر

```
npm قم بتشغيل الاختبار:منهج --block='HTML الأساسي و HTML5'
```

```
npm قم بتشغيل الاختبار:curriculum --superblock=responve-web-design
```

يمكنك أيضًا اختبار تحدي واحد فردًا من خلال تنفيذ الخطوات التالية:

1. التبديل إلى دليل 'المنهاج الدراسي`:

   ```
   منهج cd
   ```

2. قم بتشغيل ما يلي لكل ملف من ملفات التحدي التي قمت بتغيير ما يلي:

   ```
   npm اختبار -- -g 'العنوان الإنجليزي الكامل للتحدي'
   ```

بمجرد التحقق من أن كل تحدي كنت قد عملت على اجتياز الاختبارات، [يرجى إنشاء طلب سحب] (https://github.com/freeCodeCamp/freeCodeCamp/blob/Master/docs/how-to-open-a-pull-request.md).

> [!TIP]
> يمكنك تعيين متغير البيئة `LOCALE` في `.env` إلى لغة التحدي (التحديات) التي تحتاج إلى اختبار.
> 
> القيم المقبولة حاليا هي "الإنكليزية" و "chinese"، مع تعيين "english" بشكل افتراضي.

## قالب التحدي القادم

قالب التحدي في عملية التحديث إلى بنية أنظف وأقل تداخلا.  لم يتم الانتهاء من ذلك تماما، ولكن ينبغي أن يكون ما يلي قريبا من الهيكل النهائي:

``mdx

--
id: المعرف الفريد (أبجدي رقمي، MongoDB_id)
عنوان: 'عنوان التحدي'
نوع التحدي: عدد صحيح، معرف في 'العميل/Us/ChallengeTypes. s`
فيديوورل: 'عنوان URL لشرح الفيديو'
forumTopicId: 12345
---

استيراد سكريبت من './script. dx';

## --step-description--

نص الوصف، في markdown

``html
<div> 
  مثال رمز
</div>
```

## --تلميحات الخطوات--

![test-id-1]

سيكون هناك عدد اعتباطي من ثلاث مرات للمعرفات والتعليمات (في markdown) والكتل البرمجية.

```js
كود الاختبار الأول
```

![test-id-2]

المزيد من الإرشادات في بناء الجملة markdown

```js
المزيد من التعليمات البرمجية
```

## --بذرة خطوة--

### --رمز المستخدم مسبقاً--

```lang
تم تقييم الرمز قبل المستخدم
```

### --رمز المستخدم --

```lang
تم تقييم الرمز بعد المستخدم، وقبل الاختبارات مباشرة
```

### --محتوى البذورة--

![index-html]

```html
بعض html
```

```css
بعض الشارات
```

```js
بعض Js
```

![index-js]

<Script ></p>


<h1 spaces-before="0">
  --علامة الحل--
</h1>



<p spaces-before="0">
  نفس الشيء بالضبط مع قسم البذور
</p>

<h2 spaces-before="0">
  - علامة الحل التالية
</h2>



<p spaces-before="0">
  نفس الشيء مرة أخرى
</p>

<h1 spaces-before="0">
  - علامة استفهام
</h1>

<h2 spaces-before="0">
  - علامة نصية
</h2>



<p spaces-before="0">
  يطرح السؤال هنا (يستخدم فقط لتحديات الفيديو)
</p>

<h2 spaces-before="0">
  --علامات الإجابة--
</h2>



<p spaces-before="0">
  الإجابة 1
</p>

<hr />

<p spaces-before="0">
  الإجابة 2
</p>

<hr />

<p spaces-before="0">
  المزيد من الإجابات
</p>

<h2 spaces-before="0">
  --علامة الحل--
</h2>



<p spaces-before="0">
  \<number of correct answer\>
</p>



<p spaces-before="0">
  ````
</p>

<h3 spaces-before="0">
  روابط مفيدة
</h3>



<p spaces-before="0">
  تحديات خلق وتحرير:
</p>



<ol start="1">
  <li>
    <p spaces-before="0">
      <a href="https://github.com/freeCodeCamp/freeCodeCamp/blob/master/client/utils/challengeTypes.js#L1-L13">أنواع التحديات</a> - ما تعنيه قيم نوع التحدي الرقمي (عدد).
    </p>
  </li>

  
  <li>
    <p spaces-before="0">
      <a href="https://www.youtube.com/watch?v=iOdD84OSfAE#t=2h49m55s">المساهمة في FreeCodeCamp - كتابة اختبار التحدي ES6</a> - فيديو يتبع <a href="https://twitter.com/ArrowoodTech">إيثان آروود</a> لأنه يساهم في النسخة القديمة من المنهج الدراسي.
    </p>
  </li>

</ol>