# مدخل إلى المتحكمات الدقيقة Microcontrollers

نتعرف في مقال اليوم على مفهوم المتحكمات الدقيقة بشكل عام ونشرح على وجه الخصوص لوحة أردوينو بمختلف أنواعها وما الخطوات التي ستحتاجها للتعامل معها وإدخال الكود البرمجي فيها.

## ما هو المتحكم الدقيق؟

المتحكم الدقيق هو دارة متكاملة تمثل حاسوب متكامل يوجد على شريحة واحدة فهي تحتوي على جميع المكونات الرئيسية للحاسوب القياسي، وتتضمن:

+ معالج Processor: والمعالج هو الجزء الذي تتخذ فيه كل القرارات.
+ ذواكر  Memories: مساحات تخزينية وتكون من ذاكرة القراءة فقط (ROM) وذاكرة الوصول العشوائي (RAM).
+ حواف Edges:
+ مداخل ومخارج Inputs/outputs: هي وسيلة تواصل المتحكم الدقيق مع العالم الخارجي.
  

 <img src="https://github.com/abdelazizyusuf/mechatechy/raw/main/images/what-is-microcontroller1-1.png" alt="مكونات المتحكمات الدقيقة" width="300"  >


طورت إنتل أول معالج على شريحة single-chip processor  عام 1971 تحت اسم إنتل 4004. وكانت وحدة المعالجة المركزية (CPU) لهذا المعالج تعمل بنظام 4 بت. لاحقًا تطورت الأمور بسرعة كبيرة وطُورت الكثير من المعالجات التي استخدمت في العديد من الأجهزة مثل الحواسيب والهواتف والشاشات وغيرها من الأجهزة الذكية فكل هذه الأجهزة تعتمد على المعالجات أو المتحكمات الدقيقة لتعمل.

## الفرق بين المعالجات والمتحكمات الدقيقة

لعلك تتساءل ما الفرق بين المعالج أو حدة المعالجة المركزية CPU وبين المتحكم الدقيق microcontroller؟ وإليك الجواب باختصار المتحكمات الدقيقة هي معالجات لكنها مصغرة وتستهلك موارد أقل  من المعالجات الحاسوبية فهي أقل حجمًا وتكلفة واستهلاكًا للطاقة. وهي مناسبة لتصميم لبرامج المضمنة التي تتحكم في الأجهزة المختلفة مثل محركات السيارات، وأجهزة التحكم عن بعد والطابعات والأدوات المنزلية، وألعاب الأطفال والهواتف الخلوية وغيرها الكثير من الأجهزة من حولنا والتي يطلق عليها عادة أجهزة [انترنت الأشياء iot](https://abdelazizyusuf.github.io/mechatechy/2022/11/12/iot.html).

<img src="https://github.com/abdelazizyusuf/mechatechy/raw/main/images/cpu-v-microporcessor.png" alt="الفرق بين المعالجات الدقيقة والمتحكمات" width="300" >



## أنواع المتحكمات الدقيقة

هناك أنواع عديدة من المتحكمات الدقيقة وأكثرها شيوعًا هي عائلة لوحات أردوينو Arduino فهي تستخدم لتطوير المشاريع الطلابية وكلمة Arduino هي مصطلح تجميعي لوصف نوع مختلف من تصميمات اللوحات، وكل ما هو مصنوع باستخدام معالج Atmel AVR.

ستجد أنواعًا كثيرة من لوحات أردوينو تناسب مختلف أنواع المشاريع، وتكمن الاختلافات الرئيسية بين لوحات Arduino على اختلاف تسمياتها بما يلي:

+ نوع المعالج
+ عدد منافذ الدخل والخرج
+ الشكل الخارجي
+ الأداء

حيث تتمتع بعض لوحات أردوينو Arduino بذاكرة كبيرة و سرعة الحساب، وبعضها يحتوي على عدد أكبر من المدخلات / المخرجات مثل لوحة Arduino Mega كما أن بعضها مصمم للاستخدام في مشاريع معقدة وهناك لوحات تتضمن موصلات إيثرنت Ethernet أو وحدات بلوتوث Bluetooth

السحر الكامن وراء هذه العائلة هو حقيقة أنه يمكننا استخدام نفس بيئة التطوير المتكاملة (IDE) على أجهزة الحاسوب الخاصة بنا لبرمجة أي من تلك اللوحات.

## أشهر أنواع لوحات أردوينو

+ أردوينو أونو Arduino Uno
+ أردوينو ميغا Arduino Mega 2560
+ أردوينو ليلي باد Arduino LilyPad
+ أردوينو نانوArduino Nano
+  أردوينو ميغا Arduino Mega

 يمكنك برمجة هذه اللوحات من خلال العديد من المنصات وأطر العمل مفتوحة المصدر وبالعديد من لغات البرمجة مثل C أو ++C  أو لغات البرمجة القائمة على النقر مثل Pure Data لنظام التشغيل ويندوز كما يمكنك استعمال بيئة التطوير المتكاملة IDE التي توفر واجهة سهلة الاستخدام حيث يمكنك كتابة التعليمات البرمجية الخاصة بك باستخدام لغة برمجة أردوينو، وهي نسخة مبسطة من لغة C++. كما يمكنك ترجمة وتحميل التعليمات البرمجية الخاصة بك إلى لوحة أردوينو الخاصة بك، مما يؤدي فعليًا إلى نقل التعليمات من جهاز الكمبيوتر الخاص بك إلى اللوحة.
  التعليمات البرمجية التي تكتبها تشبه وصفة طبية أو مجموعة تعليمات للوحة أردوينو الخاصة بك. إنها تخبر اللوحة ما هي أجهزة الاستشعارالتي يجب قراءة البيانات منها (على سبيل المثال، درجة الحرارة، الضوء) وكيفية معالجة تلك البيانات وما هي المخرجات (على سبيل المثال، المصابيح، المحركات)

لتنفيذ البرامج تحتاج لشراء لوحة أردوينو وكابل USB لوصل اللوحة بجهاز الحاسوب الخاص بك وإضاءة LED وشاشة قراءة وغيرها من الإلكترونيات التي يتطلبها مشروعك.

ومن أهم الأشياء التي تحتاج لفهمها لبرمجة اللوحات هي طريقة إنشاء المخططات أو النماذج الأولية prototyping التي توصف المشروع بدقة على سبيل المثال إذا كنت تريد برمجة مشروع للتحكم بإضاءة LED عليك رسم مخطط بلوحة Arduino ومصباح LED الخاص بك وتوضيح كيفية يتم توصيلهما معًا.

## خطوات التعامل مع لوحات أردوينو


<img src="https://github.com/abdelazizyusuf/mechatechy/raw/main/images/what-is-microcontroller1-2.png" alt="خطوات التعامل مع أردوينو"  >


لجعل لوحة أردوينو Arduino تعمل بالشكل المطلوب عليك بداية وصف المشروع أو خطوات العمل التي تريد اتباعها بدقة فالوصف المفصل الدقيق هو مفتاح نجاح مشروعك.

بعد وصف المشروع ابدأ برسم مخطط لبوصل الدارة الإلكترونية، وابدأ بتوصيل المكونات المادية (الأجهزة) بلوحة أردوينو الخاصة بك. تتضمن هذه الخطوة  تجميع الدارة والتي تتكون من توصيل لوحة أردوينو بمكونات إلكترونية أخرى باستخدام أسلاك ومكونات إلكترونية مثل أجهزة الاستشعار (على سبيل المثال، مستشعرات درجة الحرارة، مستشعرات الضوء) والمشغلات (على سبيل المثال، المصابيح، المحركات) والمقاومات (للتحكم في تدفق التيار) ولوحات توصيل (للمساعدة في تثبيت المكونات وتوصيلها مؤقتًا)

من الأفضل الاعتماد في توصيل اللوحة على مخطط رسومي يُظهر كيفية توصيل المكونات، والتأكد من التوصيلات الصحيحة، بعدها عليك كتابة التعليمات البرمجية الخاصة بك لجعل المكونات تعمل وتحميلها للوحة، دقق في لوحة Arduino الخاصة بك، سترى دائرة متكاملة مستطيلة باسم ATMEL هذا هو المعالج وهو المكان الذي سيحتوي على البرنامج بأكمله الذي سنعيد كتابته والذي سيجعل الأشياء تعمل.

تخيل أنك تبني مشروعًا بسيطًا يقوم بتشغيل مصباح LED عند الضغط على زر معين عندها تحتاج لأن تقوم بالتالي:

+ كتابة التعليمات البرمجية في بيئة تطوير أردوينو المتكاملة، وتخبر اللوحة بأن تستمع لضغط الزر (قراءة المدخلات) إذا تم الضغط على الزر شغل مصباح LED
+  توصيل الزر ومصباح LED بلوحة أردوينو باستخدام الأسلاك، باتباع مخطط تخطيطي يوضح دبابيس التوصيل المحددة لكل مكون.
+  رفع التعليمات البرمجية للوحة وتختبر عملها وتصحح أي أخطاء برمجية


<img src="https://github.com/abdelazizyusuf/mechatechy/raw/main/images/what-is-microcontroller1-3.png" alt="Bootloader" width="300" >


تتضمن لوحة أردوينو نوعين من البرامج الأول هو برنامج الإقلاع Bootloader يكون محمل مسبقًا على اللوحة والثاني هو برنامج ثنائي ثابت binary firmware وهو البرنامج المضمن المستخدم لبرمجة اللوحة كما نريد.

## برامج مفيدة للتعامل مع لوحات أردينو

+ [برامج تشغيل FTDI USB](https://www.ftdichip.com/old2020/Drivers/VCP.htm) لتوفير الاتصال بين الحاسوب الخاص بك ولوحة Arduino
+ + بيئة تطوير أردوينو المتكاملة ([IDE](https://www.arduino.cc/en/software)):
+ [منصة Processing](https://processing.org/download/) وهي منصة معالجة مفتوحة المصدر تسهل ربط البرامج بلوحة أردوينو  وتساعدك في إنشاء مشاريع إبداعية تفاعلية في الرسومات والصوت والفيديو والألعاب وغيرها
+ ويمكن أن ترى أمثلة عدية على منصة معالجة برامج على [الرابط التالي](https://processing.org/examples/)
