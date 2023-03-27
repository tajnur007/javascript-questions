<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png">
  <h1>জাভাস্ক্রীপ্ট প্রশ্ন</h1>

---

<span>আমি আমার [ইনস্টাগ্রাম](https://www.instagram.com/theavocoder) **স্টোরিতে** জাভাস্ক্রীপ্টের মাল্টিপল চয়েজ প্রশ্ন পোস্ট করি, যেগুলো আমি এখানেও পোস্ট করবো! সর্বশেষ সংষ্করণ: <a href=#20200612><b>১২ জুন</b></a>

বেসিক থেকে এডভান্স পর্যন্ত: আপনি জাভাস্ক্রিপ্ট কতটা ভালো জানেন তা পরীক্ষা করুন, আপনার জ্ঞানকে কিছুটা রিফ্রেশ করুন বা আপনার কোডিং ইন্টারভিউয়ের জন্য প্রস্তুত করুন! :muscle: :rocket: আমি নিয়মিত নতুন প্রশ্ন সহ এই রিপো আপডেট করি। আমি প্রশ্নগুলির নীচে **collapsed section**-এ উত্তরগুলি যোগ করেছি, এটিকে expand করতে কেবল সেগুলিতে ক্লিক করুন৷ এটা শুধু মজার জন্য, শুভকামনা! :heart:</span>

নির্দ্বিধায় আমার সাথে যোগাযোগ করতে পারেন! 😊 <br />
<a href="https://www.instagram.com/theavocoder">ইনস্টাগ্রাম</a> || <a href="https://www.twitter.com/lydiahallie">টুইটার</a> || <a href="https://www.linkedin.com/in/lydia-hallie">লিংকন্ডইন</a> || <a href="https://www.lydiahallie.dev">ব্লগ</a>
</div>

| যেকোন প্রজেক্টে নির্দ্বিধায় আপনি এগুলো ব্যবহার করতে পারেন! 😃  আমি এই রিপোতে একটি রেফারেন্স পেতে খুব উপকৃত হব, আমি প্রশ্ন এবং ব্যাখ্যাসমূহ তৈরি করি (হ্যাঁ, আমি দুঃখিত লল) এবং কমিউনিটি আমাকে খুব সহায়তা করে এটি রক্ষণাবেক্ষণ এবং উন্নয়ন করতে! 💪🏼 ধন্যবাদ এবং মজা করুন!  |
|---|

---

<details><summary><b> ২০টি অনুবাদ দেখুন 🇸🇦🇪🇬🇧🇦🇬🇧🇩🇪🇪🇸🇫🇷🇮🇩🇯🇵🇰🇷🇳🇱🇧🇷🇷🇺🇹🇭🇹🇷🇺🇦🇻🇳🇨🇳🇹🇼</b></summary>
<p>

- [🇸🇦 العربية](../ar-AR/README_AR.md)
- [🇪🇬 اللغة العامية](../ar-EG/README_ar-EG.md)
- [🇧🇦 Bosanski](../bs-BS/README-bs_BS.md)
- [🇬🇧 English](../README.md)
- [🇩🇪 Deutsch](../de-DE/README.md)
- [🇪🇸 Español](../es-ES/README-ES.md)
- [🇫🇷 Français](../fr-FR/README_fr-FR.md)
- [🇮🇩 Indonesia](../id-ID/README.md)
- [🇮🇹 Italiano](../it-IT/README.md)
- [🇯🇵 日本語](../ja-JA/README-ja_JA.md)
- [🇰🇷 한국어](../ko-KR/README-ko_KR.md)
- [🇳🇱 Nederlands](../nl-NL/README.md)
- [🇧🇷 Português Brasil](../pt-BR/README_pt_BR.md)
- [🇷🇺 Русский](../ru-RU/README.md)
- [🇹🇭 ไทย](../th-TH/README-th_TH.md)
- [🇹🇷 Türkçe](../tr-TR/README-tr_TR.md)
- [🇺🇦 Українська мова](../uk-UA/README.md)
- [🇻🇳 Tiếng Việt](../vi-VI/README-vi.md)
- [🇨🇳 简体中文](../zh-CN/README-zh_CN.md)
- [🇹🇼 繁體中文](../zh-TW/README_zh-TW.md)

</p>
</details>

---

###### ১. আউটপুট কি হবে?

```javascript
function sayHi() {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

- A: `Lydia` এবং `undefined`
- B: `Lydia` এবং `ReferenceError`
- C: `ReferenceError` এবং `21`
- D: `undefined` এবং `ReferenceError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

ফাংশনের মধ্যে, আমরা প্রথমে `var` কীওয়ার্ড ব্যবহার করে `name` ভেরিয়েবল ডিক্লেয়ার করেছি। এর মানে হলো যে, ভেরিয়েবলটি `undefined` ডিফল্ট মান নিয়ে হোয়েস্টিং হয়েছে (ক্রিয়েশান ফেজ (creation phase) এর সময় মেমোরি স্পেস সেট আপ করা হয়), যতক্ষণ না আমরা আসলে সেই লাইনে না যাই যেখানে আমরা ভেরিয়েবলটিকে ডিফাইন করেছি। আমরা ভেরিয়েবলটিকে এখনও লাইনে ডিফাইন করিনি যেখানে আমরা `name` ভেরিয়েবলটিকে লগ করার চেষ্টা করেছি, তাই এটি এখনও `undefined` মান ধরে রাখে।

`let` (এবং `const`) কীওয়ার্ড ব্যবহার করে যে ভেরিয়েবলগুলো ডিক্লেয়ার করা হয় সেগুলোও হোয়েস্টিং হয় কিন্তু `var` এর মতো ইনিশিয়ালাইজ হয় না। সেগুলোকে আসলে আমরা যে লাইনে ডিক্লেয়ার করেছি তার আগে অ্যাক্সেস করা যায় না। এটাকে "temporal dead zone" বলা হয়। আমরা যখন ভেরিয়েবলগুলিকে ডিক্লেয়ার করার আগেই অ্যাক্সেস করার চেষ্টা করি তখন জাভাস্ক্রিপ্ট `ReferenceError` দেয়।

</p>
</details>

---

###### ২. আউটপুট কি হবে?

```javascript
for (var i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}

for (let i = 0; i < 3; i++) {
  setTimeout(() => console.log(i), 1);
}
```

- A: `0 1 2` এবং `0 1 2`
- B: `0 1 2` এবং `3 3 3`
- C: `3 3 3` এবং `0 1 2`

<details><summary><b>Answer</b></summary>
<p>

#### উত্তর: C

জাভাস্ক্রিপ্টে ইভেন্ট কিউ-এর কারণে, লুপটি কার্যকর হওয়ার পরে `setTimeout` কলব্যাক ফাংশনটি কল করা হয়। যেহেতু প্রথম লুপে `i` ভেরিয়েবলটি `var` কীওয়ার্ড ব্যবহার করে ডিক্লেয়ার করা হয়েছিলো, সেহেতু এই মানটি ছিল গ্লোবাল মান। লুপ চলাকালীন সময়ে আমরা ইউনারি অপারেটর `++` ব্যবহার করে প্রতিবার `i` এর মান `1` করে বৃদ্ধি করেছি। সেসময়ে `setTimeout` কলব্যাক ফাংশনটি কল হয়, প্রথম উদাহরণে তখন `i` এর মান `3` ছিলো।

দ্বিতীয় লুপে, `let` কীওয়ার্ড ব্যবহার করে `i` ভেরিয়েবলটি ডিক্লেয়ার করা হয়েছিল: `let` (এবং `const`) কীওয়ার্ড ব্যবহার করে ডিক্লেয়াার করা ভেরিয়েবল গুলো ব্লক-স্কোপড হয়ে থাকে (একটি ব্লক হল `{ }` এর মধ্যে যেকোনো কিছু)। প্রতিটি ইটারেশনের সময়, `i`-এর একটি নতুন মান থাকবে এবং প্রতিটি মান লুপের ভিতরে স্কোপ করা হবে।

</p>
</details>

---

###### ৩. আউটপুট কি হবে?

```javascript
const shape = {
  radius: 10,
  diameter() {
    return this.radius * 2;
  },
  perimeter: () => 2 * Math.PI * this.radius,
};

console.log(shape.diameter());
console.log(shape.perimeter());
```

- A: `20` এবং `62.83185307179586`
- B: `20` এবং `NaN`
- C: `20` এবং `63`
- D: `NaN` এবং `63`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

মনে রাখবেন যে `diameter` এর মান একটি রেগুলার ফাংশন, যেখানে `perimeter` এর মান একটি অ্যারো ফাংশন।

অ্যারো ফাংশনের মাধ্যমে, `this` কীওয়ার্ডটি তার বর্তমান আশেপাশের স্কোপকে বোঝায়, যা রেগুলার ফাংশনের বিপরীত! এর মানে হল, যখন আমরা `perimeter` কল করি তখন এটি shape অবজেক্টকে বোঝায় না, তবে এর আশেপাশের স্কোপকে বোঝায় (উদাহরণস্বরূপ window)।

সেই অবজেক্টটিতে `radius` নামে কোনো মান নেই, যা `NaN` রিটার্ন করে।

</p>
</details>

---

###### ৪. আউটপুট কি হবে?

```javascript
+true;
!'Lydia';
```

- A: `1` এবং `false`
- B: `false` এবং `NaN`
- C: `false` এবং `false`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

ইউনারী প্লাস অপারেটর একটি অপারেন্ডকে সংখ্যায় রূপান্তর করার চেষ্টা করে। `true` হলো `1`, এবং `false` হলো `0`।

`'Lydia'` স্ট্রিংটি একটি truthy মান। আমরা আসলে যেট জিজ্ঞাসা করেছি, "এই সত্য মানটা কি মিথ্যা?"। এটি `false` রিটার্ন করে।

</p>
</details>

---

###### ৫. কোনটি সত্য?

```javascript
const bird = {
  size: 'small',
};

const mouse = {
  name: 'Mickey',
  small: true,
};
```

- A: `mouse.bird.size` সঠিক নয়
- B: `mouse[bird.size]` সঠিক নয়
- C: `mouse[bird["size"]]` সঠিক নয়
- D: সবগুলোই সঠিক

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

জাভাস্ক্রিপ্টে অবজেক্টের সকল কী হল স্ট্রিং (যদি না এটি একটি প্রতীক হয়)। যদিও আমরা সেগুলিকে স্ট্রিং হিসাবে টাইপ নাও করতে পারি, সেগুলি ভিতরে ভিতরে সর্বদা স্ট্রিং-এ রূপান্তরিত হয়।

জাভাস্ক্রিপ্ট স্টেটমেন্টগুলিকে ইন্টারপ্রেট (বা আনবক্স) করে। যখন আমরা ব্রাকেট নোটেশন ব্যবহার করি, তখন এটি প্রথম ওপেন ব্রাকেট `[` দেখে এবং এটি ক্লোজিং ব্রাকেট খুঁজে না পাওয়া পর্যন্ত চলতে থাকে `]`। তবেই স্টেটমেন্টটিকে ইভালুয়েট করা হবে।

`mouse[bird.size]`: প্রথমে এটি `bird.size` ইভালুয়েট করে, যার মান `"small"`। `মাউস["small"]` স্টেটমেন্টটি `true` রিটার্ন করে।

যাইহোক, ডট নোটেশনের ক্ষেত্রে এটি ঘটবে না। `mouse` এর `bird` নামক কোনো কী নেই, অর্থাৎ `mouse.bird` এর মান হলো `undefined`। তারপর, আমরা ডট নোটেশন ব্যবহার করে `size` চেয়েছি: `mouse.bird.size`। যেহেতু `mouse.bird` এর মান `undefined` সেহেতু আমরা আসলে `undefined.size` এর মান চেয়েছি। এটি সঠিক নয় এবং এজন্য `Cannot read property "size" of undefined` এধরনের একটি এরর দিবে।

</p>
</details>

---

###### ৬. আউটপুট কি হবে?

```javascript
let c = { greeting: 'Hey!' };
let d;

d = c;
c.greeting = 'Hello';
console.log(d.greeting);
```

- A: `Hello`
- B: `Hey!`
- C: `undefined`
- D: `ReferenceError`
- E: `TypeError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

জাভাস্ক্রিপ্টে, সকল অবজেক্ট একে অপরের সমান সেট করার সময় _রেফারেন্স_ দ্বারা ইন্টারঅ্যাক্ট করে।

প্রথমত, ভেরিয়েবল `c` একটি অবজেক্টের মান ধরে রাখে। পরে আমরা ঐ একই রেফারেন্সের সাথে `d` কে অ্যাসাইন করি যা `c` অবজেক্টে আছে।

<img src="https://i.imgur.com/ko5k0fs.png" width="200">

এক্ষেত্রে যখন আপনি কোন একটি অবজেক্টকে পরিবর্তন করেন তখন আসলে আপনি সবগুলোকেই পরিবর্তন করেন।

</p>
</details>

---

###### ৭. আউটপুট কি হবে?

```javascript
let a = 3;
let b = new Number(3);
let c = 3;

console.log(a == b);
console.log(a === b);
console.log(b === c);
```

- A: `true` `false` `true`
- B: `false` `false` `true`
- C: `true` `false` `false`
- D: `false` `true` `true`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

`new Number()` একটি বিল্ট-ইন ফাংশন কনস্ট্রাক্টর। যদিও এটি দেখতে একটি সংখ্যার মতো, এটি আসলে সংখ্যা নয়: এটিতে বেশ কিছু অতিরিক্ত বৈশিষ্ট্য রয়েছে এবং এটি একটি অবজেক্ট।

যখন আমরা `==` অপারেটর (ইকুয়ালিটি অপারেটর) ব্যবহার করি, তখন এটি শুধুমাত্র একই _মান_ আছে কিনা সেটা চেক করে। তাদের উভয়েরই `3` এর মান আছে, তাই এটি `true` রিটার্ন করে।

যাইহোক, যখন আমরা `===` অপারেটর (স্ট্রিক্ট ইকুয়ালিটি অপারেটর) ব্যবহার করি, তখন মান _এবং_ টাইপ একই হওয়া উচিত। এটা নয়: `new Number()` কোনো সংখ্যা নয়, এটি একটি **object**। উভয়ই `false` রিটার্ন করে।

</p>
</details>

---

###### ৮. আউটপুট কি হবে?

```javascript
class Chameleon {
  static colorChange(newColor) {
    this.newColor = newColor;
    return this.newColor;
  }

  constructor({ newColor = 'green' } = {}) {
    this.newColor = newColor;
  }
}

const freddie = new Chameleon({ newColor: 'purple' });
console.log(freddie.colorChange('orange'));
```

- A: `orange`
- B: `purple`
- C: `green`
- D: `TypeError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

`colorChange` ফাংশনটি স্ট্যাটিক। স্ট্যাটিক মেথডগুলি শুধুমাত্র সেই কনস্ট্রাক্টরের মধ্যে ব্যবহার করার জন্য ডিজাইন করা হয়েছে যেখানে তাদেরকে তৈরি করা হয়েছে এবং কোন children এর কাছে এই মেথডগুলিকে পাঠানো হয় না বা ক্লাস ইনস্ট্যান্স হিসাবে কল করা যায় না। যেহেতু `freddie` হল Chameleon ক্লাসের একটি ইনস্ট্যান্স সেহেতু ফাংশনটিকে এটার সাথে কল করা যাবে না। একটি `TypeError` দেখাবে।

</p>
</details>

---
