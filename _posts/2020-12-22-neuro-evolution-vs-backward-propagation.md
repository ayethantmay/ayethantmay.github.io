---
title: 'Neuro-Evolution Vs Backward Propagation'
date: 2020-12-22
permalink: /posts/2020/12/neuro-evolution-vs-backward-propagation/
tags:
  - artificial intelligence
  - machine learning
  - reinforcement learning
  - deep learning
  - optimization
  - evolutionary computing
  - genetic algorithm
---

ပြီးခဲ့တဲ့အပတ်အတွင်းကပဲ ကျွန်မရဲ့ thesis advisor သင်တဲ့အတန်းတစ်တန်းအတွက်ကို ဒီစာသင်နှစ်ဝက်အတွက်စစ်တဲ့နောက်ဆုံးစာမေးပွဲဖြေရပါတယ်။ အဲ့အတန်းက Applied Machine Learning in Robotics ဘာသာရပ်ဖြစ်ပါတယ်။ robotics ဆိုပေမယ့် hardware ဘာသာရပ်မဟုတ်ပဲ pac man လိုဂိမ်းမျိုးလေးကိုဘာသာရပ်အစထဲက algorithm မျိုးစုံသုံးပြီး train ရပါတယ်။ robot လို့ခေါ်ရမဲ့ pac man ထဲကအကောင်မျိုးလေးက အတားအဆီးတွေကြားထဲကနေပြီး food ကိုရအောင်လိုက်စားရတာမျိုးပေါ့။

စစချင်းအပတ်မှာလုပ်ရတာက rule-based ပါ။ ပြီးတာနဲ့ နောက်အပတ်မှာ fuzzy logic ကိုစထည့်ရပါတယ်။ နောက်အပတ်ကျတော့ အဲ့ထည့်ထားပြီးသား fuzzy rules တွေကို Genetic Algorithm သုံးပြီး evolve လုပ်ခိုင်းပါတယ်။ နောက်အပတ်တွေမှာတော့ Naive Bayes နဲ့ တစ်ခါ reinforcement learning နဲ့တစ်ခါ shallow neural network နဲ့တစ်ခါ train ရပါတယ်။ ခေါင်းစဉ်တစ်ခုကို implementation အတွက်၂ ပတ်အချိန်ပေးပါတယ်။ ဘယ်အပတ်မှာ ဘာ algorithm အမျိုးအစားနဲ့ပဲ train လုပ်လုပ် ဂိမ်းရဲ့ goal ကတော့ food ကိုအချိန်တိုအတွင်း သူ့ဟာသူရအောင်ရှာနိုင်လား? ပြီးရင် food ဘယ်နှစ်ခုထိရအောင်စားနိုင်လဲ? စတာတွေပါ။ အဲ့အခါမှာ မတူညီတဲ့ algorithm တိုင်းကတော့ တူညီတဲ့ goal ကိုရောက်အောင်သွားကြတာချင်းတူပေမယ့် အလုပ်လုပ်ပုံတွေ မတူကြပါဘူး။ computational power ယူပုံချင်းလည်း မတူကြပါဘူး။ အဲ့လိုနဲ့ပဲ နောက်ဆုံးစာမေးပွဲမှာရော ဆရာဘာလုပ်ခိုင်းမလဲကို ရင်တမမ ဖြစ်ရပါတယ်။ ...

နောက်ဆုံးစာမေးပွဲရောက်လာပါပြီ။ မေးခွန်းက neuro-evolution နဲ့လုပ်ပါတဲ့။ အချိန်က ၂ ပတ်ခွဲတောင် ပေးထားပါတယ်။ အဲ့မှာ ကိုယ့်သူငယ်ချင်းနဲ့ ကိုယ်နဲ့ တိုင်စပတ်ပါပြီ။ လုပ်ရမယ့် သီးဆစ်အတွက် proposal defense နဲ့ ဆရာ့စာမေးပွဲ deadline က၂ ရက်ပဲခြားပါတယ်။ (လောင်ကြဘီလေ..) neuro-evolution ဘယ်ဆီနေမှန်းမသိပေမယ့် နှစ်ယောက်သားက neuro ဆိုတာ artificial neural network (ANN) ကိုပြောတာ နဲ့ evolution ဆိုတာ genetic algorithm (GA) ကိုရည်ညွှန်းကြောင်းဆိုတာလေးတော့ သိနေသေးလို့ ဘယ်နားဘာသွားလုပ်ရမလဲတော့ အချိန်မှီလေး သိနိုင်လိုက်ခဲ့ပါတယ်။ 😂

အဲ့လိုနဲ့ အဲ့အပတ်က neuro-evolution ကို စလေ့လာရာကနေစပြီး အလုပ်တွေ တစ်ဖြတ်ပြီးသွားတဲ့ နောက်မှာ ဒီ post ကိုရေးဖို့ အကြောင်းဖန်လာတာပဲဖြစ်ပါတယ်။ neuro-evolution အကြောင်းကိုမရေးခင်မှာ ရင်းနှီးသင့်တဲ့ အရာလေး ၃ခု ရှိနေသေးလို့ အဲ့တာလေး ၃ခုရဲ့ အကျဉ်းချုံးအကြောင်းကို အရင်ရေးချင်ပါတယ်။ ဘာတွေလဲဆိုတော့ ၁) optimization ၂) evolutionary computing ၃) backward propagation ပါ။

၁) optimization

optimization လို့ပြောလိုက်ရင် deep learning နဲ့ မစိမ်းတဲ့ စတင်လေ့လာသူတွေကတော့ neural network တွက်ချက်မှုတွေရဲ့အဆုံးသတ်မှာ အမှန်ဆုံးအဖြေထွက်လာအောင်လို့ neural network ရဲ့ parameters တွေကို တွက်ချက်မှုတစ်ခေါက်ပြီးတိုင်း ပြန်ပြန် ပြုပြင်ယူတယ်လို့ပြေးမြင်ကြလိမ့်မယ်။ အဲ့ဒါမှန်ပါတယ် ဒါပေမယ့် optimization ဘာသာရပ် ရဲ့ ဦးတည်ချက်၊ သဘော သဘာဝ၊ အမျိုးအစား တွေအားလုံးကို ခြုံငုံနိုင်ဖို့တော့ နည်းနည်းလိုနေပါသေးတယ်။ အဲ့တာကြောင့် optimization ဘာကြောင့်လိုတယ် ဘယ်လိုနေရာမှာအသုံးချတယ်ဆိုတာကနေ ဒီနေရာမှာ စပြောချင်ပါတယ်။

optimization လုပ်တယ်ဆိုတာကတော့ function တစ်ခုခုကထွက်လာတဲ့ အဖြေကို ကိုယ်လိုချင်တဲ့ အနေအထားထိရောက်အောင် မဖြစ်ဖြစ်တဲ့နည်းနဲ့ ပြုပြင်ယူတာမျိုးပါ။ အဲ့ function ကို objective function (တစ်နည်းအားဖြင့်) optimization problem ကြီးတစ်ခုလုံးရဲ့ ရည်ရွယ်ချက်လို့ ခေါ်ပါတယ်။ ဥပမာ FedEx တို့ DHL တို့လို လုပ်ငန်းမျိုးအတွက် google OR ကပေးတဲ့ service လိုမျိုး vehicle route optimization လုပ်ကြမယ်ဆိုရင် စဉ်းစားရမယ့် objective တွေရှိပါတယ်။ အဲ့တာတွေက ဒီလို vehicle route optimization လုပ်လိုက်ခြင်းအားဖြင့်
objective ၁) ပစ္စည်းတွေပို့ဖို့အတွက် ကားနဲ့သွားလာစရိတ် နည်းနိုင်သမျှ အနည်းဆုံးဖြစ်လာရမယ်။ (minimizing the total travel cost)
objective ၂) ပစ္စည်းတွေပို့ဖို့အတွက် သုံးရတဲ့ကားအရေအတွက် နည်းနိုင်သမျှ အနည်းဆုံးဖြစ်လာရမယ်။ (minimizing the number of vehicles used)
objective ၃) ဒီ service ကိုသုံးနေတဲ့ customer တွေက ဒီ service အပေါ်မှာ ကျေနပ်အားရမှု အတိုင်းအတာတစ်ခုထိတက်လာရမယ်။ (maximizing the customer satisfaction)
ဒီလိုမျိုး objective (ရည်ရွယ်ချက်) တွေ ၁ ခုထက်မကရှိနေပြီး အဲ့ objective တွေကို တစ်ပြိုင်နက်ထဲ ဖြေရှင်းခြင်းကို multiple objective optimization လို့ခေါ်ပါတယ်။ objective တစ်ခုပဲရှိတဲ့ ပြဿနာတွေကိုတော့ single objective optimization လို့ခေါ် ပါတယ်။

ပြန်ကြည့်ကြမယ်ဆိုရင် objective ဘယ်နှစ်ခုရှိရှိ အကျဉ်းချုပ်ကတော့ ၂ မျိုးပဲရှိပါတယ်။ အနည်းဆုံးကိုရှာချင်တဲ့ ရည်ရွယ်ချက် (minimization problems) နဲ့ အများဆုံးကိုရှာချင်တဲ့ ရည်ရွယ်ချက် (maximization problems) ပဲဖြစ်ပါတယ်။ အဲ့တာကြောင့် optimization လုပ်ပြီလို့ပြောလိုက်ရင် အနည်းဆုံးကိုရှာနေတာနဲ့ အများဆုံးကိုရှာနေတာဆိုပြီး ၂ ခုပဲထွက်လာပါတော့တယ်။

အဲ့တာဆိုရင် neural network optimization ကိုပြန်စဉ်းစားကြည့်ရအောင်။ neural network optimization problem ဟာဆိုရင် objective ၁ ခုပဲရှိတဲ့ single objective optimization သာဖြစ်ပါတယ်။ ဘာလို့လဲဆိုရင် သူ့ရဲ့ objective function က prediction loss / error function တစ်ခုသာဖြစ်ပါတယ်။ loss / error လို့ပြောပြီဆိုထဲက အနည်းဆုံးကိုပဲရှာရတော့တာပေါ့။ အဲ့တော့ minimization problem ဖြစ်နေပါတယ်။

၂) evolutionary computing

များသောအားဖြင့် optimization problem တွေဟာ NP-hard problem တွေများပါတယ်။ သင့်တော်တဲ့ အချိန်တစ်ခုအတွင်းမှာ အကောင်းဆုံးဆိုတဲ့ အဖြေတစ်ခုရအောင် ဖြေရှင်းဖို့ခက်ခဲတဲ့ပြဿနာမျိုးတွေပါ။ များသောအားဖြင့် အဲ့လိုပြဿနာတွေကို meta-heuristic algorithm တွေနဲ့ ဖြေရှင်းကြတာများပါတယ်။ (ဒီနေရာမှာ meta-heuristics တွေအကြောင်းကိုတော့ အသေးစိတ်မရေးပါဘူး) အဲ့လို algorithm တွေက အကြမ်းဖျင်းအားဖြင့် ထင်ရှားတဲ့ artificial intelligence ဆိုင်ရာ algorithm အုပ်စုကြီး ၂ စုထဲမှာပါပါတယ်။ ပထမအုပ်စုကတော့ ရေထဲအုပ်စုလိုက်ကူးနေတဲ့ ငါးတွေ၊ ကောင်းကင်မှာ အုပ်လိုက်ပျံနေတဲ့ ငှက်တွေ အင်းဆက်တွေ ရဲ့ သဘာဝကို တုပပြီးထုတ်ထားတဲ့ swarm intelligence လို့ခေါ်တဲ့ algorithm အုပ်စုတွေဖြစ်ပါတယ်။ ဒုတိယအုပ်စုကတော့ လူသားတွေရဲ့ မျိုးနွယ်စုအလိုက် ဆင့်ကဲဖြစ်စဉ်တွေကို တုပထားတဲ့ Charles Darwin ရဲ့ evolutionary theory ကိုအခြေခံတဲ့ evolutionary computing လို့ခေါ်တဲ့ algorithm အုပ်စုတွေဖြစ်ပါတယ်။

Genetic Algorithm ဟာ meta-heuristics တွေထဲကမှ evolutionary computing အုပ်စုဝင် algorithm တစ်ခုဖြစ်ပါတယ်။ GA အကြောင်းကို အသေးစိတ်ပြောရင် ပို့စ်အရမ်းရှည်သွားမှာစိုးလို့ အကြမ်းဖျင်းသာပြောသွားပါမယ်။ GA က optimization problem တွေအတွက် အကောင်းဆုံးအဖြေ (minimum or maximum) ကိုရှာတဲ့အခါ လူသားမျိုးနွယ်စုကြီးတစ်ခုလုံးဆင့်ကဲပြောင်းလဲလာသလိုပဲ တစ်နည်းနည်းနဲ့ ရွေးချယ်ထားတဲ့ ပဏာမ အဖြေအုပ်စုကြီး (အဖြေအုပ်စုကြီးလို့ပြောတဲ့အတွက် အဖြေတစ်ခုထဲမဟုတ်ပါ။) တစ်ခုလုံးကို ဆင့်ကဲပြောင်းလဲတာပါ။ မျိုးဆက်တစ်ဆက်ပြီးတစ်ဆက် ပိုမိုကောင်းမွန်တဲ့ မျိုးရိုးဗီဇတွေကို လက်ဆင့်ကမ်းပြီး ဆင့်ကဲပြောင်းလဲသလိုပဲ GA ဟာလည်း iteration / generation တစ်ခုပြီးတစ်ခု သူ့ရဲ့ solution တွေကိုကောင်းသထက်ကောင်းလာအောင် သတ်မှတ်ထားတဲ့ objective function နဲ့အညီ ပြုပြင်ယူပါတယ်။ နောက်ဆုံး iteration အပြီးမှာတော့ အဖြေအုပ်စုကြီးထဲက အကောင်းဆုံးအဖြေတစ်ခုကိုသာ နောက်ဆုံးအဖြေအဖြစ်ယူပါတယ်။

၃) backward propagation

ဒါနဲ့တော့ သိပ်စိမ်းကြမှာမဟုတ်ပါဘူး။ backward propagation ကတော့ neural network optimization အတွက်ကို အသုံးများပြီး အလွန်အသုံးဝင်တဲ့ နည်းပညာတစ်ခုဖြစ်ပါတယ်။ သူ့ကိုဘာကြောင့်သုံးရလဲဆိုရင် neural network တွေရဲ့ parameters ပေါင်းစုံကို 3D plane ပေါ်မှာ plot ဆွဲကြည့်မယ်ဆိုရင် မျက်နှာပြင်ကြီးက မညီမညာနဲ့ ဖြစ်ချင်တိုင်းဖြစ်နေပါတယ်။ အဲ့မျက်နှာပြင်ကြီးကို optimization surface လို့ခေါ်ပါတယ်။ အဲ့ optimization surface ကြီးရဲ့ အနိမ့်ဆုံးအပိုင်းလေးကတော့ ကိုယ်တွေလိုချင်တဲ့ global minimum error လေးပဲရှိတဲ့နေရာလေးပေါ့။ ဒီနေရာမှာ global minimum လို့ဘာလို့ပြောလဲဆိုရင် local minimum တွေလည်းရှိနေလို့ပါ။ local minimum ဆိုတာကတော့ optimization surface တစ်ခုလုံးမှာ minimum အဖြစ်ဆုံးမဟုတ်ပဲ သူ့အနီးအနားလေးတစ်ဝိုက်မှာပဲ ကွက်ပြီး minimum ဖြစ်နေတာမျိုးပါ။ optimization problem တိုင်းရဲ့ goal က global minimum or global maximum ကိုပဲရှာရတာပါ။

အဲ့တော့ backward propagation နည်းက အဲ့ global minimum error ကို optimization surface ကြီးပေါ်မှာဘယ်လိုရှာလဲဆိုရင် ဒီတိုင်းကြုံရာစမှတ်တစ်ခုယူလိုက်ပါတယ်။ အဲ့ကနေပြီး direction တစ်ခုယူပြီး တောက်လျှောက် ရှေ့ကိုဆက်သွားပါတယ်။ ဒီနေရာမှာ minimum error လေးရှိတဲ့ချိုင့်ဝှမ်းကြီးကိုရောက်မရောက်သိနိုင်ဖို့ slope (gradient descent) ကိုတွက်ယူဖို့လိုလာပါတယ်။ အဲ့ slope အတိုင်းပဲ တရွေ့ရွေ့ဆင်းပြီး လိုက်ရှာပါတယ်။ အဲ့အတွက် တစ်ခါတစ်လေ global minimum ကိုရောက်မယ်မရောက်မယ် အာမခံချက်မပေးနိုင်ပါဘူး။ local minimum မှာပဲ လမ်းဆုံးသွားတာမျိုးလည်း ရှိနိုင်ပါတယ်။

Main Topic:
neuro-evolution VS backward propagation

neuro-evolution ဆိုတာကတော့ neural network တွေကို ခုနက သမားရိုးကျ backward propagation နည်းလမ်းနဲ့ optimization လုပ်တာမဟုတ်ပဲနဲ့ backward propagation နေရာမှာ genetic algorithm လို evolutionary algorithm တွေကို အစားထိုးပြီး optimization လုပ်တာပဲဖြစ်ပါတယ်။ သူ့ကိုအကျယ်တဝင့် ဖော်ပြထားတာကတော့ Uber ရဲ့ AI research blog post နဲ့ OpenAI ရဲ့ blog post တွေမှာ real-world use case တွေအနေနဲ့ အကျယ်တဝင့်ဖတ်နိုင်ပါတယ်။ link တွေကို ပို့စ်အဆုံးမှာ ထည့်ပေးထားပါတယ်။

ဒါဆိုရင် backward propagation ရှိနေရဲ့သားနဲ့ ဘာလို့ neuro-evolution ကို လူတွေ စိတ်ဝင်စားလာနေရလဲဆိုတာလည်း နည်းနည်းပြောချင်ပါတယ်။ data ပမာဏတွေ များပြားလာပြီးတော့ deep learning ခေတ်စားလာတဲ့နောက်မှာ သမားရိုးကျ supervised learning, သမားရိုးကျ unsupervised learning, သမားရိုးကျ reinforcement learning တွေနေရာမှာ deep learning ကဝင်ရောက်လာပါတယ်။ အဲ့အခါမှာ deep neural network တွေရဲ့ကဏ္ဍက အရင်ကထက်ပိုပြီး အပြောများလာကြပါတယ်။

supervise learning အတွက် DNN က optimize လုပ်ရမယ့် objective function ကတော့ loss function ဖြစ်ပါတယ်။ loss function ကို လျှော့ချချင်နေတာဖြစ်တဲ့အတွက် minimization problem ပါ။ supervised learning မှာ label / class တွေရှိပါတယ်။ ဆိုလိုချင်တာက အဖြေတစ်ခုတွက်ကြည့်ပြီးရင် မှန် မမှန် ပြန်ချိန်ကိုက်ဖို့အတွက် စံနမူနာအဖြေတွေရှိပါတယ်။ အဲ့အဖြေတွေပေါ်မူတည်ပြီး loss / error function ကို အတိအကျတွက်လို့ရပါတယ်။ သမားရိုးကျ supervised learning နေရာကို deep neural networks (DNNs) တွေအစားဝင်တဲ့အခါမှာ backward propagation နည်းလမ်းက အရမ်းအသုံးဝင်ပါတယ်။ တိကျတဲ့အဖြေတစ်ခုရှိပြီးသားဖြစ်တဲ့အတွက် အဲ့အဖြေပေါ်မူတည်ပြီး slope ရှာတဲ့အခါမှာ global minimum ကို အတတ်နိုင်ဆုံးရောက်အောင်သွားနိုင်ပါတယ်။

ဒါဆိုရင် reinforcement learning ကိုစဉ်းစားကြည့်ရအောင်။ reinforcement learning ရဲ့ objective function က supervised learning နဲ့မတူပါဘူး။ loss function မဟုတ်ပဲ reward function ဖြစ်ပါတယ်။ reward function လို့ပြောတဲ့အတွက် reward များလေ ရှာချင်တဲ့အဖြေ ပိုကောင်းလေ ဖြစ်တဲ့အတွက် maximization problem ဖြစ်ပါတယ်။ ဒါပေမယ့် reinforcement learning ဘက်ကို DNN တွေအစားဝင်တဲ့အချိန်မှာတော့ backward propagation နည်းလမ်းမှာ ပြဿနာအနည်းငယ်ရှိပါတယ်။ reinforcement learning မှာ supervised learning တုန်းကလို စံနမူနာအဖြေအတိကျရှိမနေပါဘူး။ ဒီ state ရောက်ရင် ဒီ action လုပ်ဖို့ probability ဘယ်လောက်ရှိမယ်။ အိုခေ.. အဲ့ action လုပ်လိုက်တယ်ဆိုရင် သူ့ကို reward ဘယ်လောက်ပေးလိုက်မယ်ဆိုတာ အတိအကျမရှိပါဘူး။ လူက DNN ကို ကြိုပြီး reward ဘယ်လောက်ထည့်ပေးလိုက်ဆိုပြီး ခန့်မှန်းပေးထားတာသာဖြစ်ပါတယ်။ အဲ့တော့မြင်ယောင်ကြည့်ပါ။ backward propagation သုံးမယ်ဆိုရင် gradient descent ခမျာလည်း စမ်းတဝါးဝါးနဲ့ လည်နေဖို့ အလားအလာတွေများနေပါပြီ။

အဲ့လိုနဲ့ backward propagation လိုမျိုး single solution တစ်ခုထဲ စမ်းတဝါးဝါးနဲ့ လျှောက်ရှာနေရတဲ့နည်းလမ်းအစား solution တွေ အများကြီးကို တစ်ပြိုင်နက်ထဲထုတ်၊ ဆင့်ကဲပြောင်းလဲခိုင်းပြီး အကောင်းဆုံးကိုရှာကြည့်တော့တာပေါ့။ အဲ့အတွက်ကြောင့် reinforcement learning ပြဿနာမျိုးမှာ deep learning အစားဝင်မယ်ဆိုရင် traditional backward propagation နဲ့မရှင်းပဲ evolutionary computing နဲ့ရှင်းရင် ရလာဒ်များ ပိုကောင်းလာမလားဆိုပြီး စရာကနေ neuro-evolution က reinforcement learning နယ်ပယ်အတွက်ကို အလားအလာရှိတဲ့ research တစ်ခုဖြစ်လာပါတော့တယ်။

ရလာဒ်တွေကလည်း အတော်ကောင်းကောင်းပါ။ ဒါပေမယ့် မကောင်းတာတွေလည်းရှိပါတယ်။ ထုံးစံအတိုင်းပေါ့ xP ... အဲ့တာကတော့ computational power ပါ။ backward propagation ထက်အများကြီး power ပိုလိုပါတယ်။ ဒါပေမယ့် cloud computing ထွန်းကားလာတဲ့အတွက် အဲ့နောက်မှာ neuro-evolution ကတော့ အလားအလာရှိတဲ့ စိတ်ဝင်စားဖို့လည်း အတော်ကောင်းတဲ့ သုတေသန နယ်ပယ်တစ်ခုဖြစ်လာနေပါတယ်။

References:
-----
1. [OpenAI](https://openai.com/blog/evolution-strategies/)
2. [Uber AI Research](https://eng.uber.com/deep-neuroevolution/)
