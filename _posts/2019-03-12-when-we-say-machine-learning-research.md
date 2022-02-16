---
title: 'When We Say Machine Learning Research'
date: 2019-03-12
permalink: /posts/2019/03/when-we-say-machine-learning-research/
tags:
  - machine learning
  - research
  - data
  - data science
---

မရှင်းလမ်းနင်း သုတေသန (Machine Learning Research) ဆိုတာက algorithm တွေများကြီးသိပြီး Python တွေ R တွေရေးတတ်သွားတာနဲ့ဘာမှတော့မဆိုင်ပါ။ ကိုယ့် data ကိုမကြည့်တတ်ရင် အလကားပါပဲ။ data ကိုကြည့်တတ်တယ် မကြည့်တတ်ဘူးဆိုတာကို အလွယ်ကူဆုံး ဥပမာတွေပေးရရင်

ဥပမာ (၁) continuous numerical data ပေါ်မှာ prediction လုပ်ချင်နေတာကို Regression လိုမျိုးကိုမသုံးဘဲ categorical data ပေါ်မှာလုပ်တဲ့ Classification ကိုသုံးမယ်လို့ စဉ်းစားတာမျိုးပါ။ ဒီနေရာမှာ Regression ကို မသုံးချင်ဘူးဆိုလည်း neural network အမျိုးအစားထဲက Multiple Layer Perceptron ကိုသုံးလို့ရပါသေးတယ်။ တစ်ခုရှိတာက neural network တွေမှာ feature variables တွေဟာ interaction ရှိပါတယ်။ Linear Regression မှာတော့အဲ့လိုသဘောတရားမရှိပါဘူး။

ဥပမာ (၂) ကိုယ့် data ရဲ့အနေအထား ပမာဏက deep learning သုံးစရာမလိုအပ်သေးပဲ statistics ဘက်ကပဲဖြေရှင်းလို့ရနေတဲ့အနေအထားမျိုးမှာ deep learning သုံးမယ်ဆိုရင် အပ်နဲ့ထွင်းရမှာကိုပုဆိန်နဲ့ပေါက်သလိုဖြစ်နေပါ။ ( deep learning ဆိုတာ လက်ရှိမှာ highly active area of research ပါ။ ဒါပေမယ့်အဲ့အဓိပ္ပါယ်က deep learning သုံးမှ neural network မှာ hidden layers တွေထပ်ထပ်ထည့်မှခေတ်မှီတာလို့ယူဆရမည့်အရာ မဟုတ်ပါ။ neural network ထဲမှာ hidden layer ၂ ခုလောက်ထည့်တိုင်းလည်း deep learning ဖြစ်သွားတာမဟုတ်ပါ။ neural network သုံးတိုင်း မ deep ပါ။ )

ဥပမာ (၃) use case ၁ ခုအနေနဲ့ card fraud detection/ transaction fraud detection လိုပြဿနာမျိုးကို supervised learning အတိုင်းဖြေရှင်းမယ်လို့စဉ်းစားကြည့်ကြမယ်ဆိုရင် neural network သုံးရေး logistic regression သုံးရေး random forest လို ensemble methods တွေသုံးရေးသည်ပြဿနာမဟုတ်ပါ။ ပြဿနာက supervised learning ဖြစ်တဲ့အတွက် class ၂ ခုရှိပါတယ်။ Non-fraud နဲ့ fraud ပါ။ အဲ့ class ၂ ခုဟာ imbalance ဖြစ်ပါတယ်။ အဓိပ္ပါယ်က fraud class ရဲ့ ratio ဟာ dataset ရဲ့ 0.01 လောက်ဖြစ်ပြီး non fraud class က 0.99 လောက်ဖြစ်နေတာမျိုးပါ။ အရေအတွက် မမျှတဲ့သဘောပါ။ ဘာလို့လဲဆိုတော့ လူတိုင်းပြဿနာမရှာပါ ( ဆိုလိုချင်တာက လူတိုင်း fraud မလုပ်ပါ။ ) အလွန်နည်းတဲ့ လူနည်းစုသာလုပ်လို့ပါ။ :3 အဲ့လိုအချိန်မျိုးမှာ algorithm မလာခင် class တွေညီအောင် resampling methods တွေလိုမျိုးတွေသုံးဖို့လိုပါတယ်။
Unsupervised Learning သုံးမယ်ဆိုလည်း outlier detection လုပ်ဖို့အတွက် data ကိုကြည့်တတ်ဖို့လိုပါတယ်။ ဘာလို့လဲဆိုရင် abnormal behavior ရှိတဲ့ outliers တိုင်းသည် fraudulent actions မဟုတ်ပါ။

ဥပမာ (၄) data ကိုသဘောပေါက်သွားလို့ algorithm အဆင့်ပြီးသွားလို့ model ၁ ခုထွက်ရင်တောင်မပြီးသေးပါဘူး။ Parameter Tuning တွေ method evaluation တွေရှိပါသေးတယ်။ evaluation ဆိုတာလည်း accuracy နဲ့ပဲ တိုင်းတာတာမျိုးမဟုတ်ပါ။ တစ်ချို့ပြဿနာတွေ အတွက် accuracy metric ကအဆင်ပြေပေမယ့်တစ်ချို့ပြဿနာတွေအတွက် precision ကပိုအဆင်ပြေတာမျိုး recall ကပိုသင့်တော်တာမျိုးရှိပါသေးတယ်။ ( precision, recall, f-measure အကြောင်းသိချင်ရင် confusion matrix ကို အရင်နားလည်အောင်လုပ်သင့်ပါတယ်။ )

ဒီဥပမာတွေကအကုန်မဟုတ်သေးပါဘူး။ အရမ်းကိုအခြေခံအဆင့်မှာပဲရှိပါသေးတယ်။

Python တွေ R တွေဆိုတဲ့ programming language တွေဆိုတာ ကိုယ်သုံးချင်တဲ့ algorithm တွေ metric တွေ class တွေကိုခေါ်သုံးဖို့ tools ၁ ခုအပြင်မပိုပါဘူး။ ဘယ် algorithm ကို ဘယ် data ပေါ်မှာသုံးသင့်တယ်ဆိုတာသိရင်ဘယ်သူမဆို အချိန်မရွေးခေါ်သုံးလို့ရပါတယ်။ python မှာလည်း library တွေ framework တွေမျိုးစုံရှိပါတယ်။ scikit-learn မှ tensorflow မှ pytorch မှရယ်လို့မဟုတ်ပါ။ ကိုယ်နဲ့သင့်တော်ရာအဆင်ပြေရာသုံးနိုင်ပါတယ်။ OCR အတွက်ဆိုလည်း tesseract တွေဘာတွေ ရှိပါသေးတယ်။ General application တစ်ခုရယ်လို့မြန်မြန်နဲ့ကောင်းကောင်း ထွက်ချင်တာပါပဲဆိုရင်တော့လည်းမခဲယဉ်းပါ။ pre-trained models တွေ pre-built models တွေလိုတောင်ယူသုံးလည်းထွက်ပါတယ်။ ( pre-trained နဲ့ pre-built လည်းမတူပါ။ google ရဲ့ VisionAPI သည် pre-trained ဖြစ်ပြီး google ရဲ့ AutoML သည် pre-built ပါ။ ) တခြား alternative automated open sourced machine learning library တွေလည်းရှိပါသေးတယ်။ ဥပမာဆိုရင် Auto Keras ။ အဲ့လိုမျိုးတွေသုံးထားတယ်ဆိုရင်တော့ ဒီလိုတွေစဉ်စားရချင်မှစဉ်းစားရမှာပါ။ ဒါပေမယ့်သူ့နေရာနဲ့သူတော့ကောင်းကျိုး ဆိုးကျိုးတွေ limitation တွေတော့ရှိတာကြီးပါပဲ။ (အဲ့လိုပြောတာက coding က လျစ်လျူရှုရမယ့်အရာမဟုတ်ပါဘူး။ production အဆင့်မှာတင်မဟုတ်ပဲ prototype အဆင့်မှာပါအတိုင်းအတာတစ်ခုထိအရေးပါပါတယ်။ သုတေသနရှုထောင့်ကရေးတဲ့အတွက် သုတေသနအတွက်လိုအပ်ဆုံးရှုထောင့်ကိုပဲထုတ်ရေးခြင်းဖြစ်ပါတယ်။ coding ကတော့ သုတေသနအဆင့်မှာ ၁၀၀% မဟုတ်ပေမယ့်လည်းအတိုင်းအတာတစ်ခုထိတော့အရေးပါနေတယ်ဆိုတာ မေ့လို့မရပါဘူး။)

machine learning ဆိုတာ data science ရဲ့ tools လို့ပြောလို့ရပါတယ်။ ML/ DL ကိုသေချာလုပ်နိုင်ချင်ရင်တော့ data science ရဲ့သဘောကိုသေချာသိဖို့လိုကိုလိုပါတယ်။ data ဆိုတာ any data ပါ။ image, audio, text, numeric, tabular ကြိုက်တာဖြစ်နိုင်ပါတယ်။ အဲ့တော့ ပြန်ပြောရမယ်ဆိုရင် Machine Learning Research ဆိုတာ အရေးပါတဲ့idea ထွက်အောင်အရင်စဉ်းစားရမယ့်အစား သုတေသနအတွက် လိုအပ်ဆုံးရှုထောင့်တွေကို မေ့ပစ်ပြီးတော့ ဘာ language သုံးမယ် ဘာ framework သုံးမယ်ပြီးအရင်လုပ်နေရမှာမဟုတ်ပါဘူး။ 😁😁