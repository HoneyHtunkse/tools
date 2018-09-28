# Example usages of perl programs

## clean-space.pl

```bash
lar@lar-air:~/tool/perl$ cat ./tst-input 
This is  a car.
  This is       a cat.


cat is a cat.     

Blue

B l     u           e    


lar@lar-air:~/tool/perl$ perl ./clean-space.pl ./tst-input 
This is a car.
This is a cat.
cat is a cat.
Blue
B l u e
lar@lar-air:~/tool/perl$
```

## rmEnglishSentences.pl

```bash
lar@lar-air:~/tool/perl$ cat tst-input2
မြန်မာစာ နဲ့ English
မြန်မာစာ နဲ့ အင်္ဂလိပ်စာ
ကခဂ နဲ့ abc
ကခဂ နဲ့ အေဘီစီ
Do you speak English?
အင်္ဂလိပ်စကား ပြောနိုင်လား။

ဘာလုပ်နေတာလဲ။ thinking လုပ်နေတာလား။
က a ခ b ဂ c
a b c d e f g
lar@lar-air:~/tool/perl$ perl ./rm-EnglishSentences.pl ./tst-input2 
မြန်မာစာ နဲ့ အင်္ဂလိပ်စာ
ကခဂ နဲ့ အေဘီစီ
အင်္ဂလိပ်စကား ပြောနိုင်လား။
```
## word-analysis.pl

```bash
lar@lar-air:~/tool/perl$ ./word-analysis.pl ./10-lines 
4 word(s) sentence(s) : 
	10 : ၇ နာရီ ပါ ။
total: 1

6 word(s) sentence(s) : 
	3 : ညစာ က ဘယ် အချိန် လဲ ။
total: 1

9 word(s) sentence(s) : 
	9 : ဥပမာ ရောန်ဂွန်း ကို ရန်ကုန် ဟု အစားထိုး ခဲ့ သည် ။
total: 1

11 word(s) sentence(s) : 
	7 : မျူနီစီပယ် ရပ်ကွက် ၃၈ ၊ အိမ်ခြေ ပေါင်း ၃၅ဝဝဝ ခန့် ရှိ ၏ ။
total: 1

19 word(s) sentence(s) : 
	8 : အမည်ရင်း ကိုလှ ဖြစ် ပြီး ၂၆ စက်တင်ဘာ ၁၉၁၇ တွင် ပုစွန်တောင် ရေကျော်ရပ် ၌ ဦးဖိုးထင် ဒေါ်သင်းမြိုင် တို့ က ဖွားမြင် ခဲ့ သည် ။
total: 1

21 word(s) sentence(s) : 
	2 : ဗိုင်ဩလိုဂျီ သည် သက်ရှိ အရာ သို့မဟုတ် သဇီဝ တို့ နှင့် ပတ်သက် သော အကြောင်း အကျိုး တို့ ကို လေ့လာ သော သိပ္ပံ ပညာရပ် ဖြစ် သည် ။
total: 1

27 word(s) sentence(s) : 
	5 : GOS တွက်ချက် ရန် စုစုပေါင်း ထုတ်လုပ် မှု စရိတ် မှ ကုန်ကျငွေ တစ်စိတ်တစ်ပိုင်း ကို သာ နုတ်ယူ တွက်ချက် ထား ခြင်း ဖြစ် သော်လည်း သာမန် အားဖြင့် အမြတ်စွန်း ရရှိ သည့် ငွေ ဖြစ် သည် ။
total: 1

32 word(s) sentence(s) : 
	6 : တွေ့ဆုံ ရာတွင် ဗိုလ်ချုပ် အောင်ဆန်း သည် မိမိ ကိုယ် မိမိ မြန်မာ နိုင်ငံ ယာယီ အစိုးရ ၏ ကိုယ်စားလှယ် အဖြစ် မိတ်ဆက် ပြီး ၊ မဟာမိတ် စစ် ဦးစီး တစ် ဦး အဖြစ် အသိအမှတ်ပြု ရန် ရဲရဲတင်းတင်း တောင်းဆို လိုက် ပါ သည် ။
total: 1

34 word(s) sentence(s) : 
	1 : စိုက်ပျိုး ရေး သည် နိုင်ငံ ၏ အဓိက လုပ်ငန်း ဖြစ် သော်လည်း များပြား သော လူဦးရေ ၏ စား ဝတ် နေ ရေး ဖူလုံ စေရန် အိန္ဒိယ နိုင်ငံ သည် စက်မှု နိုင်ငံ အဖြစ် သို့ အရှိန် ကောင်းကောင်း ဖြင့် ချီတက် လျက် ရှိ သည် ။
total: 1

35 word(s) sentence(s) : 
	4 : အစော ဆုံး ခိုင်မာ သည့် သမိုင်း အထောက်အထား မှာ ၁၅၈၆ ၁၅၈၈ အတွင်း မြန်မာ နိုင်ငံ သို့ ရောက် ရှိ လာ ခဲ့ သည့် အင်္ဂလိပ် လူမျိုး ခရီးသွား RalphFitch ၏ မှတ်တမ်း ဖြစ် ပြီး ၎င်း က Cosmin မြို့ ဟု မှတ်သား ခဲ့ သည် ။
total: 1

Average words per line : 19.80
lar@lar-air:~/tool/perl$ ./word-analysis.pl ./10-lines -longest-shortest
lar@lar-air:~/tool/perl$ ./word-analysis.pl ./10-lines longest-shortest
Longest sentence : 35 words
	4 : အစော ဆုံး ခိုင်မာ သည့် သမိုင်း အထောက်အထား မှာ ၁၅၈၆ ၁၅၈၈ အတွင်း မြန်မာ နိုင်ငံ သို့ ရောက် ရှိ လာ ခဲ့ သည့် အင်္ဂလိပ် လူမျိုး ခရီးသွား RalphFitch ၏ မှတ်တမ်း ဖြစ် ပြီး ၎င်း က Cosmin မြို့ ဟု မှတ်သား ခဲ့ သည် ။
total : 1


Shortest sentence : 4 word(s)
	10 : ၇ နာရီ ပါ ။
total : 1

Average words per line : 19.80
lar@lar-air:~/tool/perl$ ./word-analysis.pl ./10-lines count
4 word(s) : 1 sentence(s)
6 word(s) : 1 sentence(s)
9 word(s) : 1 sentence(s)
11 word(s) : 1 sentence(s)
19 word(s) : 1 sentence(s)
21 word(s) : 1 sentence(s)
27 word(s) : 1 sentence(s)
32 word(s) : 1 sentence(s)
34 word(s) : 1 sentence(s)
35 word(s) : 1 sentence(s)
Average words per line : 19.80
```