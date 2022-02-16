---
title: 'Python or PowerBI? Which one you need'
date: 2019-12-21
permalink: /posts/2019/12/python-powerbi/
tags:
  - data analysis
  - business intelligence
  - data science
  - python
  - power bi
  - tableau
---

ကြားနေကြ ကြုံနေကြ "Power BI သုံးလေ Python လိုလို့လား?" ဆိုတာမှာ မေးစရာမေးခွန်း ၂ ခုရှိပါတယ်။

၁) Power BI သုံးချင်တဲ့လူက Power BI ဘာလဲဆိုတာ သေချာသိလား?
၂) Python သုံးချင်တဲ့လူက ဘာအတွက် python ကိုသုံးချင်တာလဲ? Data visualization က dashboard တွေအတွက်လား ၊ data management အတွက်လား ၊ data science အတွက်လိုချင်တဲ့ stats/DL library တွေသုံးချင်လို့လား?

အဲ့တာတွေကိုမဆွေးနွေးခင်မှာ Data Analysis နဲ့ Data Science ကိုတူတယ်ထင်ပါသလား မထင်ပါဘူးလားနဲ့စပါရစေ။ အဲ့ ၂ခုက တကယ်တော့မတူပါဘူး။ တူရင်နာမည်ပါတူတူပေးလိုက်သင့်ပါတယ်။ (joking 😛) မတူတဲ့အတွက် အလုပ်လုပ်တဲ့လူတွေရဲ့ position တွေလည်းမတူပါဘူး။ data analyst နဲ့ data scientist မတူပါဘူး။

Data analysis ဟာ data science ရဲ့ preprocessing အဆင့်တွေထဲမှာပြန်ပါတယ်လို့ ပြောရင်လည်းမှားမယ်မထင်ပါဘူး။ data ကို clean လုပ်ရမယ်။ (ဒီနေရာမှာ ကိုယ့် data ပေါ်မူတည်ပြီး လုပ်ရမယ့် အဆင့်တွေထပ်ရှိပါဦးမယ်) report တွေကို end user တွေပြန်ပြရမယ်။ Data analysis အတွက် report sheet တွေ dashboard တွေ chart တွေကို excel file မှာလည်း လုပ်လို့ရသလို snowflake တို့ BigQuery တို့လို Warehouse တွေ (warehouse ကဆို ETL တွေ scheduler တွေရှိလိမ့်မယ်) MySQL လို RDBMS တွေ MongoDB လို N-RDBMS တွေ csv လို file တွေကြိုက်တဲ့ data source ပေါ်မှာလုပ်လို့ ဆွဲလို့ရပါတယ်​။ ပြီးရင် ဆွဲထားတဲ့ chart တွေကို end user ကိုပြမယ်။ ဒါတွေကို business intelligence(BI) လို့လည်း နောက်တစ်မျိုး ခေါ်ပါသေးတယ်။

Power BI ဆိုတာက microsoft ကစီးပွားဖြစ်ထုတ်ထားတဲ့ BI tool ၁ ခုပါ။ Tool လို့ပြောတဲ့အတွက် code ရေးစရာမလိုပဲ သူ့ပစ္စည်းသုံးရုံနဲ့ BI (data analysis) လုပ်လို့ရပါတယ်။ data privacy ကိုလည်း sensitive မဖြစ်ဘူး။ ကိုယ့်လိုအပ်ချက်နဲ့လည်းကိုက်တယ်။ တန်ရာတန်ကြေးလည်းတတ်နိုင်တယ်ဆို license တွေဝယ်ပြီးသုံးကြပါတယ်။ အချိန်ကုန်သက်သာ လူကုန်သက်သာ UI/UX လည်းပြောစရာမရှိလို့ပါ။ ဒီထက်တတ်နိုင်ရင် Tableau သာသွားသုံးပါလေ။ UX မှာ power BI ထက်ပိုစိတ်ကျေနပ်စရာကောင်းပါတယ်။ power BI ထက်လည်း elite function တွေပိုပါတယ်။ စျေးကလည်းပိုကြီးပါတယ်။

Data analysis အကြောင်းကို သိသလောက်လေး ပြောကြည့်ပြီးပြီဆိုတော့ data science အကြောင်းကိုလည်း ပြောချင်ပါသေးတယ်။ data science ဟာ data analysis ထက်ပိုပြီးနက်နဲပါတယ်။ ရှုပ်ထွေးပါတယ်။ အခုနက analysis လုပ်ပြီးသား data တွေကိုသုံးပြီး Business problems တွေထဲက insights တွေကိုရှာတဲ့နေရာမှာ သုံးပါတယ်။ (ဒီ ပို့စ်က business field အတွက်ပဲရေးလို့ပါ။ တကယ်က မတူညီတဲ့ field တွေပေါ်မှာ data science ကိုလုပ်ကြပါတယ်။ အခြေခံသဘောတရားကတော့ တူတူပဲဖြစ်ပါတယ်)။ ဥပမာ အနေနဲ့ Customer Churn Prediction လုပ်မယ် Market segmentation လုပ်မယ် Customer Lifetime Value (CLTV) ကိုကြည့်မယ်။ report ထုတ်တာထက် ဒီလိုရှုပ်ထွေးသွားတဲ့ ပြဿနာတွေကို data analysis ကမဖြေရှင်းပေးနိုင်ပါဘူး။ Analysis လုပ်ထားတဲ့ data တွေကို အသုံးပြုပြီး data science ကဘဲ ဖြေရှင်းပေးနိုင်ပါတယ်။ ဒါဆိုရင်ဘာကြောင့် science လို့ပြောရသလဲကို နည်းနည်းမြင်ပြီလို့မျှော်လင့်ပါတယ်။ အပေါ်ကပြဿနာတွေအတွက် တိကျတဲ့ solution ပေးနိုင်ဖို့ကို ဖြေရှင်းနိုင်မယ့် method အမျိုးမျိုးနဲ့ ကိုယ့် data ပေါ်မှာ စမ်းကြည့်ပြီး အကောင်းဆုံး အဖြေပေးနိုင်တဲ့ method ကိုယူရပါတယ်။ ဒါကြောင့် science လို့ခေါ်ပါတယ်။

အဲ့ဒီအခါမှာ လက်တွေ့စမ်းသပ်ဖို့အတွက် programming language ဆိုတာလိုလာပါတယ်။ အဲ့အတွက်ကို Python ကိုသုံးကြပါတယ်။ (Python မှာက data science အတွက်အသုံးပြုရမယ့် machine learning library တွေ statistical library တွေ deep learning framework တွေ resource ကြွယ်လို့ပါ)။ algorithm တွေဟာ အဲ့ဒီ python library ထဲမှာရှိနေတဲ့အတွက် ကိုယ့်ဟာကို အစကနေ (from scratch) လုပ်နေစရာ တွက်ချက်နေစရာမလိုလို့ပါ။ ပြီးသွားရင် တွက်ချက်ထားတဲ့ အဖြေတွေမှန်မမှန်ကို ထုတ်ကြည့်ဖို့လိုပါတယ်။ ဒီမှာ visualization လိုလာပြန်ပါတယ်။ တကယ်တော့ data ရဲ့ variantion ကြည့်ချင်တာ dimension ကြည့်ချင်တာ accuracy လိုမျိုး result metric တွေကြည့်ချင်တာလောက်နဲ့ visualization ကို Power BI တွေ Tableau တွေသုံးစရာမလိုပါ။ Matplotlib တို့ Bokeh တို့လို python library တွေနဲ့ပဲခြေနိုင်လက်နိုင်ကြည့်ကြပါတယ်။

ဒီလောက်ဆိုရင် ကိုယ်လိုချင်တာ Power BI လား Python လား data analysis လား data science လားအကြမ်းဖျင်းတော့ခွဲခြားလို့ရပါပြီ။ အခုနကလိုမျိုး "Power BI သုံးလေ Python လိုလားပြော" ဆိုတဲ့မေးခွန်းမျိုးတွေကို ဘယ်မှာမြင်ဖူးလဲဆိုရင် client တွေနဲ့ စကားပြောရင်သော်လည်းကောင်း ကိုယ် offline online သွားနားထောင်တဲ့ ပွဲမျိုးမှာ speaker လုပ်တဲ့လူကို audience ကထမေးရင်သော်လည်းကောင်း မြင်ဖူးပါတယ်။

အဲ့လိုအမေးခံရမှာ သေချာတဲ့ speaker တွေက ဘယ်လိုလူတွေလဲဆိုရင် ဥပမာ "Python for Data Science" တို့ဘာတို့ လိုမျိုး data science programming အခြေခံကို ဝေမျှချင်တဲ့ speaker တွေ ပညာရှင်တွေပါ။ သူတို့ slide မှာ accuracy ဒါမှမဟုတ် loss ကို matplotlib နဲ့ chart ဆွဲပြတဲ့နေရာရောက်တာ နဲ့ audience က "Power BI သုံးလေ Python လိုလားပြော" ဆိုတာမျိုး ထဖန်တီးပေးပါတော့မယ်လို့ပြောရင်းပဲ ဒီစာအရှည်ကြီးကိုအဆုံးသတ်ပါရစေ။