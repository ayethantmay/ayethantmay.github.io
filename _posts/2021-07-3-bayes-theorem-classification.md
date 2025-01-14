---
title: 'Bayes Theorem, Naive Bayes Classification and Generative Learning (Part - 1)'
date: 2021-07-3
permalink: /posts/2014/08/bayes-theorem-classification/
tags:
  - bayes theorem
  - naive bayes classifier
  - classification
  - generative learning
---

probability လို့ပြောလိုက်ရင် ကျွန်မတို့တွေက equation တွေကိုပဲပြေးမြင်လေ့ရှိကြပါတယ်။ အဲ့တာဘာလို့လဲဆိုရင် ကျောင်းမှာ အဲ့ equation တွေကို ကျက်ပြီးမှတ်ရတယ် ပြီးရင် စာမေးပွဲမှာ ပြန်ချရေးရတယ်။ အဲ့လိုစနစ်ထဲမှာ စာသင်လာကြရလို့ပါပဲ။ တကယ်တမ်း လက်တွေ့ဘဝမှာ ဘယ်နေရာမှာသုံးနေလဲ ဘာအတွက်ကြောင့် သူ့ကိုသုံးဖို့လိုအပ်သလဲဆိုတာကိုတွေးခေါ်နိုင်ဖို့တော့ အခြေအနေမပေးခဲ့ကြပါဘူး။ Bayes လို့ကြားလိုက်တာနဲ့ equation တွေပဲပြေးမြင်တာက ကောင်းတဲ့အလေ့အထမဟုတ်ပါဘူး (equation မှားမှတ်လဲ ပြဿနာ)။ တကယ်တမ်းမှာ Bayes လို့ကြားလိုက်တာနဲ့ ဘာပြဿနာအမျိုးအစားဆိုရင် သူနဲ့ရှင်းလို့ရတယ်လို့မြင်နိုင်မှ Bayes ကိုအသုံးပြုပုံကို မမေ့ကြတော့မှာဖြစ်ပါတယ်။

ဒီနေ့ Part - 1 မှာတော့ Bayes Theorem အကြောင်းနဲ့ပဲ အရင်စပြောကြည့်ပါမယ်။ နောက်ရက်တွေရေးမယ့် Part - 2 နဲ့ Part - 3 မှာတော့ Naive Bayes Classifier နဲ့ Generative Learning တွေအကြောင်းဆက်ရေးသွားနိုင်အောင်လုပ်ပါ့မယ်။


Bayes Theorem
------

ဥပမာဆိုပါစို့။ သင်နိုးလာတဲ့အချိန်မှာ သင့်ကိုယ်သင် နေမကောင်းဘူးလို့ စခံစားနေရပြီ။ (အနံ့ပျောက်နေတာမျိုးပေါ့ . . နောက်တာပါ) အဲ့တာနဲ့ ဆေးခန်းသွားတယ်ပေါ့။ ဘာရောဂါဆိုတာပါကို တပ်အပ်ပြောဖို့အတွက် ဆရာဝန်ကိုယ်တိုင်ကလည်း မသေချာဘူး။ ဆိုတော့ ဆေးစစ်ခိုင်းလိုက်တယ်ပေါ့။ အဲ့တာနဲ့ ရက်ပိုင်းလောက်ကြာတော့ ဆေးစစ်ချက်အဖြေထွက်လာပြီ။ အဖြေရလဒ်အရဆိုရင် သင်က လူဦးရေရဲ့ တော်တော်နည်းတဲ့ ပမာဏ (လူအယောက် ၁၀, ၀၀၀ မှာမှ ၁ ယောက်လောက်) မှာပဲ ဖြစ်လေ့ဖြစ်ထရှိတဲ့ ရောဂါအထူးအဆန်းတစ်ခုမှာ positive ဖြစ်နေတယ်ဆိုပါတော့။

အဲ့တော့သင်က ဆရာဝန်ကိုမေးမယ် ဒီ test ကြီးက ဘယ်လောက်ထိ တိကျသေချာမှုရှိလို့လဲပေါ့ (ပြန်ဖလိန်းတာပေါ့လေ 😒)။ အဲ့တော့ဆရာဝန်ကပြောရော ဒီ test က လူဦးရေရဲ့ 90% ကို အဲ့ရောဂါတကယ်ဖြစ်နေရင် တကယ်အတည်ဖြစ်နေကြောင်း (positive ဖြစ်ကြောင်း) ပြောပေးနိုင်တယ်။ ကျန်တဲ့ 10% ကိုပဲ ရောဂါတကယ်မရှိပဲနဲ့ ရှိတယ်ဆိုပြီး positive လို့မှားပြောမိနိုင်ချေရှိတယ်ပေါ့။

အဲ့မှာစဉ်းစားဖို့လိုတာက ပထမအချက်အနေနဲ့ ပုံမှန် ၁၀ ယောက်ရှိ ၈ ယောက် ၉ ယောက်လောက် ဖြစ်တတ်တဲ့ ရိုးရိုးမိုးရာသီတုပ်ကွေးလောက်။ ပြီးတော့ ဒုတိယအချက်အနေနဲ့ ဆေးတကယ်စစ်ပြီဆိုရင်လည်း အဲ့ test က ရောဂါတကယ်မရှိပဲ ရှိတယ်လို့မှားပြတဲ့ percent (false positive percent) နည်းမယ်ဆိုရင် သိပ်အများကြီး သံသယဖြစ်စရာမလိုဘူးပေါ့။

ပြောရရင်တစ်ကယ်တမ်းမှာ လူဦးရေရဲ့ ဘယ်နှစ်ယောက်ပဲရောဂါဖြစ်ဖြစ် သူ့ဟာသူနည်းနည်း များများ အဲ့တာက အရေးမဟုတ်ပါဘူး။ အဓိကက ဒုတိယအချက်ပဲ။ အဲ့တာကမှ critical system တွေရဲ့ classification accuracy ဘာကြောင့်အရမ်းများသင့်သလဲဆိုတာရဲ့ အကြောင်းအရင်းဖြစ်လာမယ်လို့ထင်မိတယ်။

ဆိုတော့ ဆေးစစ်ချက်မှာရောဂါရှိတယ်လို့ပြောတိုင်း ကိုယ်ကရောဂါတကယ်ဖြစ်နေပြီလားပေါ့။ ဘာလို့ဆိုသူ့မှာက ရောဂါတကယ်မရှိပဲနဲ့ ရှိတယ်လို့ positive ပြနိုင်ချေ 10% ချည်းများတောင် ရှိနေတာကိုး။ 😩

test က positive ပြနေတိုင်း ကိုယ့်မှာ တကယ်ရောဂါရှိတယ်ဆိုတာ ဘယ်လောက် percent ထိပဲသေချာလဲဆိုတာကို သိဖို့အတွက် Bayes Theorem ကိုသုံးပြီးတွက်ကြည့်လို့ရပါတယ်။ အဲ့တာတွက်ဖို့ဆိုရင် conditional probability ကိုမှတ်မိမယ်ထင်တယ်နော်။ Bayes က အဲ့တာနဲ့ပဲတွက်ကြည့်ရမှာဆိုတော့ နည်းနည်းပြန် intro ထည့်လိုက်ပါမယ်။

P(A) = probability of event A
P(X) = probability of event X
P(X|A) = probability of A under the condition of A
P(A|X) = probability of X under the condition of A

ရောဂါတကယ်ရှိတယ်ဆိုတဲ့ကိစ္စကို A လို့ထား။ test လိုက်တော့ positive ဖြစ်နေတယ်ဆိုတဲ့ကိစ္စကို X လို့ထားမယ်။ ဒီမှာ probability တွေအကြောင်းတော့ အသေးစိတ်မပြောတော့ပါဘူး။ အဲ့တာဆိုရင် Bayes Theorem ရဲ့ equation ကိုချရေးကြည့်တော့မယ်။

P(A|X) = P(X|A) * P(A) / P(X) ကိုပုံစံပြောင်းပြီးအောက်ကပုံစံအတိုင်းရေးပါမယ်။

P(A|X) = P(X|A) * P(A) / [P(X|A) * P(A)] + [P(X| not A) * P(not A)]
ဒီ equation ရဲ့သဘောကတော့

test ကထွက်လာတာ positive ဖြစ်နေတယ်ဆိုတဲ့ ဟာက ဘယ်လောက်မှန်သလဲဆိုတဲ့ probability P(A|X) ကိုရဖို့အတွက်

ရောဂါတကယ်ရှိနေတဲ့အချိန်မှာ test က positive ပြပေးတဲ့ probability P(X|A) ရယ်၊

လူဦးရေထဲမှာရောဂါဖြစ်လေ့ရှိတဲ့ပမာဏ P(A)ရယ်၊

ရောဂါတကယ်မရှိပဲ test က positive လို့မှားပြနေတဲ့ probability P(X| not A) ရယ်၊

လူဦးရေထဲမှာရောဂါမဖြစ်တဲ့ပမာဏ P(not A) ရယ် ကို သက်ဆိုင်ရာ ကိန်းကဏန်းတွေ အစားထိုးလိုက်ရင် လိုချင်တဲ့ အဖြေရပါပြီ။

ဆိုတော့
P(A|X) = 0.9 * 0.0001 / 0.9 * 0.0001 + 0.1 * 0.9999 = 0.00089 = 0.089% ရပါလိမ့်မယ်။

အနှစ်ချုပ်ပြောရရင်တော့ test က positive ထွက်ပေမယ့် ကိုယ့်မှာ တကယ်ရောဂါဖြစ်နေတယ်ဆိုတဲ့အဆိုက 0.089% ပဲမှန်နေတယ်ဆိုတာပါပဲ။ အဲ့လိုမဖြစ်အောင် medical နဲ့ဆိုင်တဲ့ critical system တွေအတွက်လုပ်တဲ့ classification တွေရဲ့ accuracy ကဘာကြောင့် အများကြီးဖြစ်သင့်ကြလဲဆိုတာ ဒါကြောင့်လို့ပဲထင်မိပါတယ်။

စာတော့နည်းနည်းရှည်သွားပြီ။ Part - 2 နဲ့ Part - 3 ကိုတော့ နောက်ရက်တွေကျရင် ဆက်ရေးကြည့်ပါဦးမယ်။ 😁