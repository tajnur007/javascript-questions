<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png">
  <h1>জাভাস্ক্রীপ্টের প্রশ্ন</h1>

---

<span>আমি আমার [ইনস্টাগ্রাম](https://www.instagram.com/theavocoder) **স্টোরিতে** জাভাস্ক্রীপ্টের মাল্টিপল চয়েজ প্রশ্ন পোস্ট করি, যেগুলো আমি এখানেও পোস্ট করবো! সর্বশেষ সংষ্করণ: <a href=#20200612><b>১২ জুন</b></a>

বেসিক থেকে এডভান্স পর্যন্ত: আপনি জাভাস্ক্রিপ্ট কতটা ভালো জানেন তা পরীক্ষা করুন, আপনার জ্ঞানকে কিছুটা রিফ্রেশ করুন বা কোডিং ইন্টারভিউয়ের জন্য প্রস্তুত করুন! :muscle: :rocket: আমি নিয়মিত নতুন প্রশ্ন সহ এই রিপো আপডেট করি। আমি প্রশ্নগুলির নীচে **collapsed section**-এ উত্তরগুলি যোগ করেছি, উত্তরগুলি দেখতে এটিকে ক্লিক করুন৷ এটা শুধুমাত্র মজা হিসেবে, শুভকামনা! :heart:</span>

নির্দ্বিধায় আমার সাথে যোগাযোগ করতে পারেন! 😊 <br />
<a href="https://www.instagram.com/theavocoder">ইনস্টাগ্রাম</a> || <a href="https://www.twitter.com/lydiahallie">টুইটার</a> || <a href="https://www.linkedin.com/in/lydia-hallie">লিংকন্ডইন</a> || <a href="https://www.lydiahallie.dev">ব্লগ</a>
</div>

| যেকোন প্রজেক্টে নির্দ্বিধায় আপনি এগুলো ব্যবহার করতে পারেন! 😃 আমি এই রিপোতে একটি রেফারেন্স পেলে খুবই উপকৃত হবো, আমি প্রশ্ন এবং ব্যাখ্যাসমূহ তৈরি করি এবং কমিউনিটি এটিকে রক্ষণাবেক্ষণ এবং উন্নয়ন করতে আমাকে খুব সহায়তা করে! 💪🏼 ধন্যবাদ!  |
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

<details><summary><b>উত্তর</b></summary>
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
!'Tajnur';
```

- A: `1` এবং `false`
- B: `false` এবং `NaN`
- C: `false` এবং `false`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

ইউনারী প্লাস অপারেটর একটি অপারেন্ডকে সংখ্যায় রূপান্তর করার চেষ্টা করে। `true` হলো `1`, এবং `false` হলো `0`।

`'Tajnur'` স্ট্রিংটি একটি সত্য বা truthy মান। আমরা আসলে যেটা জিজ্ঞাসা করেছি, "এই সত্য মানটা কি মিথ্যা?"। এটি `false` প্রদান করে।

</p>
</details>

---

###### ৫. কোনটা সত্য?

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

জাভাস্ক্রিপ্টে, অবজেক্টের কীগুলো হলো স্ট্রিং টাইপের (সিম্বল না হলে)। যদিও আমরা সেগুলোকে স্ট্রিং হিসেবে টাইপ করিনা, তবে ভিতরে ভিতরে সেগুলো সর্বদা স্ট্রিং হিসেবে রূপান্তরিত হয়।

জাভাস্ক্রিপ্ট স্টেটমেন্টগুলিকে ইন্টারপ্রেট (অথবা আনবক্স) করে। যখন আমরা ব্র্যাকেট নোটেশন ব্যবহার করি, তখন এটি প্রথমে ওপেনিং ব্র্যাকেটটি `[` দেখে এবং সে ক্লোজিং ব্র্যাকেটটি `]` না পাওয়া পর্যন্ত চলতে থাকে। ঠিক তখনই সে স্টেটমেন্টটিকে মূল্যায়ন করবে।

`mouse[bird.size]`: প্রথমে এটি `bird.size` স্টেটমেন্টটিকে ইভালুয়েট করবে, যার মান `"small"`। `mouse["small"]` স্টেটমেন্টটি `true` রিটার্ন করে।

তবে ডট নোটেশন দিয়ে করতে গেলে এটা এমনভাবে হতো না। `mouse` অবজেক্টটিতে `bird` নামে কোনো _কী_ (key) নেই, এর মানে `mouse.bird` এর মান `undefined`। এরপর আমরা ডট নোটেশন ব্যবহার করে `size` কে বের করতে চাই: `mouse.bird.size`। যেহেতু `mouse.bird` এর মান `undefined`, সেহেতু আমরা আসলে `undefined.size` এর মান বের করতে চাচ্ছি। এটি সঠিক নয় এবং এজন্য `Cannot read property "size" of undefined` এধরনের একটি এরর দিবে।

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

###### ৯. আউটপুট কি হবে?

```javascript
let greeting;
greetign = {}; // Typo!
console.log(greetign);
```

- A: `{}`
- B: `ReferenceError: greetign is not defined`
- C: `undefined`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

এটি অবজেক্টটিকে লগ আকারে দেখাবে কারণ আমরা আসলে গ্লোবাল অবজেক্টে একটি খালি অবজেক্ট তৈরী করেছি! যখন আমরা `greeting` কে ভুলক্রমে `greetign` হিসেবে টাইপ করি তখন জাভাস্ক্রিপ্টের ইন্টারপ্রেটার আসলে এটাকে এভাবে দেখে:

1. Node.js এ `global.greetign = {}` এভাবে।
2. ব্রাউজারে `window.greetign = {}`, `frames.geetign = {}` এবং `self.greetign` এভাবে।
3. ওয়েব ওয়ার্কার্সে `self.greetign` এভাবে।
4. সব ধরনের এনভায়রনমেন্টে `globalThis.greetign` এভাবে।

আমরা এটি এড়িয়ে চলতে `"use strict"` ব্যবহার করতে পারি। এটি নিশ্চিত করে যে আপনি যেকোনো ভেরিয়েবলে মান সেট করার আগে ভেরিয়েবলটিকে ডিক্লেয়ার করেছেন।

In order to avoid this, we can use `"use strict"`. This makes sure that you have declared a variable before setting it equal to anything.

</p>
</details>

---

###### ১০. এটা করলে কি হবে?

```javascript
function bark() {
  console.log('Woof!');
}

bark.animal = 'dog';
```

- A: কিছুই হবে না, এটা পুরোপুরি ঠিক আছে!
- B: `SyntaxError`. এই ভাবে আপনি একটি ফাংশনে প্রোপার্টি যোগ করতে পারবেন না। 
- C: `"Woof"` লগ আকারে দেখাবে।
- D: `ReferenceError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

জাভাস্ক্রিপ্টে এটা সম্ভব, কারণ ফাংশনগুলি অবজেক্ট হিসেবে ব্যবহার করা হয়! (প্রিমিটিভ টাইপের সবকিছুই অবজেক্ট)।

ফাংশন একটি বিশেষ ধরনের অবজেক্ট। আপনি আসলে যে কোড লিখেন সেটা আসলে ফাংশন নয়। ফাংশনটি একটি অবজেক্ট যার প্রপার্টিগুলি রয়েছে। এই প্রপার্টি কল করা সম্ভব।

</p>
</details>

---

###### ১১. আউটপুট কি হবে?

```javascript
function Person(firstName, lastName) {
  this.firstName = firstName;
  this.lastName = lastName;
}

const member = new Person('Lydia', 'Hallie');
Person.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};

console.log(member.getFullName());
```

- A: `TypeError`
- B: `SyntaxError`
- C: `Lydia Hallie`
- D: `undefined` `undefined`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

জাভাস্ক্রিপ্টে, ফাংশনগুলি অবজেক্ট হয় এবং এর জন্যই `getFullName` মেথডটি নিজস্ব কনস্ট্রাক্টর ফাংশন অবজেক্টে যোগ হয়। এই কারণে, আমরা `Person.getFullName()` কল করতে পারি, কিন্তু `member.getFullName` একটি `TypeError` থ্রো করে।

আপনি যদি একটি মেথডকে সব অবজেক্ট ইনস্ট্যান্সগুলিতে ব্যবহার করতে চান, তবে এটি প্রোটোটাইপ প্রপার্টিতে যোগ করতে হবে:

```js
Person.prototype.getFullName = function() {
  return `${this.firstName} ${this.lastName}`;
};
```

</p>
</details>

---

###### ১২. আউটপুট কি হবে?

```javascript
function Person(firstName, lastName) {
  this.firstName = firstName;
  this.lastName = lastName;
}

const lydia = new Person('Lydia', 'Hallie');
const sarah = Person('Sarah', 'Smith');

console.log(lydia);
console.log(sarah);
```

- A: `Person {firstName: "Lydia", lastName: "Hallie"}` এবং `undefined`
- B: `Person {firstName: "Lydia", lastName: "Hallie"}` এবং `Person {firstName: "Sarah", lastName: "Smith"}`
- C: `Person {firstName: "Lydia", lastName: "Hallie"}` এবং `{}`
- D: `Person {firstName: "Lydia", lastName: "Hallie"}` এবং `ReferenceError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

`sarah` এর জন্য আমরা `new` কিওয়ার্ড ব্যবহার করিনি। `new` কিওয়ার্ড ব্যবহার করলে `this` তখন আমরা নতুন যে খালি অবজেক্টকে তৈরী করেছি সেটাকে রেফার করে। তবে, আপনি যদি `new` কিওয়ার্ড যোগ না করেন, `this` তখন **global object** কে রেফার করে!

আমরা বলেছি `this.firstName` সমান `"Sarah"` এবং `this.lastName` সমান `"Smith"`। আসলে আমরা যেটা করেছি সেটা হলো `global.firstName = 'Sarah'` এবং `global.lastName = 'Smith'`। `sarah` এর মান ইতিমধ্যে `undefined`, কারণ আমরা `Person` ফাংশন থেকে কোনো মান রিটার্ন করিনি।

</p>
</details>

---

###### ১৩. ইভেন্ট প্রোপাগেশনের তিনটি ধাপ কি কি?

- A: Target > Capturing > Bubbling
- B: Bubbling > Target > Capturing
- C: Target > Bubbling > Capturing
- D: Capturing > Target > Bubbling

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

**capturing** ধাপে, ইভেন্টটি পূর্ববর্তী এলিমেন্ট গুলির মাধ্যমে নীচের টার্গেট এলিমেন্টে প্রবেশ করে। এরপর ইভেন্টটি **target** এলিমেন্টে পৌঁছে যায় এবং **bubbling** শুরু হয়।

<img src="https://i.imgur.com/N18oRgd.png" width="200">

</p>
</details>

---

###### ১৪. সব অবজেক্টের প্রোটোটাইপ থাকে।

- A: true
- B: false
s
<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

**base object** ব্যতিত সব অবজেক্টেরই প্রোটোটাইপ থাকে। বেস অবজেক্ট হলো ইউজার কর্তৃক তৈরি করা অবজেক্ট বা `new` কিওয়ার্ড ব্যবহার করে তৈরি করা অবজেক্ট। বেস অবজেক্টটি কিছু মেথড এবং প্রপার্টি অ্যাক্সেস করতে পারে, যেমন `.toString`। আপনি জাভাস্ক্রিপ্টের নিজস্ব মেথডগুলি ব্যবহার করতে পারেন তার কারণ এটিই! এধরনের মেথডগুলি প্রোটোটাইপে পাওয়া যাবে। যদিও জাভাস্ক্রিপ্ট আপনার অবজেক্টে এটি সরাসরি খুঁজে পায়না, এটি প্রোটোটাইপ চেইনে যায় এবং সেখানে এটি পায়, যা আপনার জন্য অ্যাক্সেসেবল করে।

</p>
</details>

---

###### ১৫. আউটপুট কি হবে?

```javascript
function sum(a, b) {
  return a + b;
}

sum(1, '2');
```

- A: `NaN`
- B: `TypeError`
- C: `"12"`
- D: `3`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

জাভাস্ক্রিপ্ট একটি **dynamically typed language**: ভেরিয়েবলগুলি কোন ধরনের হবে আমরা সেটা নির্দিষ্ট করে বলিনা। আপনাকে না জানিয়েই মানগুলি সয়ংক্রিয়ভাবে অন্য একটি টাইপে রূপান্তরিত হতে পারে, যাকে _implicit type coercion_ বলে। **Coercion** হলো একটি টাইপকে অন্য টাইপে রূপান্তর করা।

এই উদাহরণে, জাভাস্ক্রিপ্ট `1` সংখ্যাটিকে একটি স্ট্রিং-এ রূপান্তর করে, যাতে ফাংশনটি স্বাভাবিক হয়ে একটি মান ফেরত দেয়। একটি সংখ্যার টাইপ (`1`) এবং একটি স্ট্রিং টাইপ (`'2'`) যোগ করার সময়, সংখ্যাটি স্ট্রিং হিসাবে ব্যবহৃত হয়। আমরা স্ট্রিংগুলিকে `"Hello" + "World"` এভাবে যুক্ত করতে পারি, তাই এখানে আসলে যেটা ঘটতেছে সেটা হলো `"1" + "2"` যা `"12"` রিটার্ন করে।

</p>
</details>

---

###### ১৬. আউটপুট কি হবে?

```javascript
let number = 0;
console.log(number++);
console.log(++number);
console.log(number);
```

- A: `1` `1` `2`
- B: `1` `2` `2`
- C: `0` `2` `2`
- D: `0` `1` `2`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

**postfix** ইউনারি অপারেটর `++`:

১. মানটি রিটার্ন করে (এটি `0` রিটার্ন করে)
২. মানটি বৃদ্ধি করে (সংখ্যাটি এখন `1`)

**prefix** ইউনারি অপারেটর `++`:

১. মানটি বৃদ্ধি করে (সংখ্যাটি এখন `2`)
২. মানটি রিটার্ন করে (এটি `2` রিটার্ন করে)

এটি `0 2 2` রিটার্ন করে।

</p>
</details>

---

###### ১৭. আউটপুট কি হবে?

```javascript
function getPersonInfo(one, two, three) {
  console.log(one);
  console.log(two);
  console.log(three);
}

const person = 'Lydia';
const age = 21;

getPersonInfo`${person} is ${age} years old`;
```

- A: `"Lydia"` `21` `["", " is ", " years old"]`
- B: `["", " is ", " years old"]` `"Lydia"` `21`
- C: `"Lydia"` `["", " is ", " years old"]` `21`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

যদি আপনি ট্যাগড টেমপ্লেট লিটারাল ব্যবহার করেন, তবে প্রথম আর্গুমেন্টের মান সর্বদা স্ট্রিং মানগুলির একটি অ্যারে হয়। অবশিষ্ট আর্গুমেন্টগুলি পাস করা এক্সপ্রেশনগুলির মান পায়!

</p>
</details>

---

###### ১৮. আউটপুট কি হবে?

```javascript
function checkAge(data) {
  if (data === { age: 18 }) {
    console.log('You are an adult!');
  } else if (data == { age: 18 }) {
    console.log('You are still an adult.');
  } else {
    console.log(`Hmm.. You don't have an age I guess`);
  }
}

checkAge({ age: 18 });
```

- A: `You are an adult!`
- B: `You are still an adult.`
- C: `Hmm.. You don't have an age I guess`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

যখন ইকুয়ালিটি বা সমতা টেস্ট করি, প্রিমিটিভ টাইপের ডাটাগুলো তাদের _value_ দ্বারা তুলনা করা হয়, অবজেক্টের ক্ষেত্রে তাদের রেফারেন্স দ্বারা তুলনা করা হয়। জাভাস্ক্রিপ্ট চেক করে যে অবজেক্টগুলির রেফারেন্স মেমোরির একই স্থানে রয়েছে কি না।

আমরা যে দুটি অবজেক্ট তুলনা করছি তাদের ক্ষেত্রে এটি নেই: আমরা যে অবজেক্টটির সাথে ইকুয়ালিটি বা সমতা চেক করছি সেটা মেমোরিতে যে স্থানে রেফারেন্স করে আছে, প্যারামিটার হিসাবে যে অবজেক্টটি পাঠিয়েছি সেটি অন্য একটি মেমোরি স্থানে রেফারেন্স করে আছে।

এই কারণে `{ age: 18 } === { age: 18 }` এবং `{ age: 18 } == { age: 18 }` উভয়ই `false` রিটার্ন করে।

</p>
</details>

---

###### ১৯. আউটপুট কি হবে?

```javascript
function getAge(...args) {
  console.log(typeof args);
}

getAge(21);
```

- A: `"number"`
- B: `"array"`
- C: `"object"`
- D: `"NaN"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

রেস্ট প্যারামিটার (`...args`) আমাদের অবশিষ্ট সব আর্গুমেন্টগুলিকে একটি অ্যারেতে সংগ্রহ করতে দেয়। অ্যারে একটি অবজেক্ট, তাই `typeof args` এক্সপ্রেশনটি `"object"` রিটার্ন করে।

</p>
</details>

---

###### ২০. আউটপুট কি হবে?

```javascript
function getAge() {
  'use strict';
  age = 21;
  console.log(age);
}

getAge();
```

- A: `21`
- B: `undefined`
- C: `ReferenceError`
- D: `TypeError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

`"use strict"` ব্যবহার করে আপনি নিশ্চিত হতে পারেন যে আপনি ভূলেও গ্লোবাল ভেরিয়েবল ডিক্লেয়ার করেননি। আমরা কখনো `age` ভেরিয়েবলটিকে ডিক্লেয়ার করিনি, এবং এই কারণে আমরা `"use strict"` ব্যবহার করলে এটি রেফারেন্স এরর থ্রো করবে। যদি আমরা `"use strict"` ব্যবহার না করতাম, তাহলে `age` প্রপার্টি গ্লোবাল অবজেক্টে যোগ হয়ে যেতো, সে কারণেই এটি কাজ করতো।

</p>
</details>

---

###### ২১. `sum` এর মান কত?

```javascript
const sum = eval('10*10+5');
```

- A: `105`
- B: `"105"`
- C: `TypeError`
- D: `"10*10+5"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

একটি স্ট্রিং হিসাবে পাঠানো কোডকে `eval` ইভালুয়েট করে। এটি একটি এক্সপ্রেশন হলে, এক্ষেত্রে যেমনটি হয়েছে, এটি এক্সপ্রেশনটিকে ইভালুয়েট করে। এক্সপ্রেশনটি হলো `10 * 10 + 5`। এটি `105` সংখ্যাটিকে রিটার্ন করে।

</p>
</details>

---

###### ২২. কতক্ষণ পর্যন্ত cool_secret কে অ্যাক্সেস করা যাবে?

```javascript
sessionStorage.setItem('cool_secret', 123);
```

- A: ডেটা কখনো হারিয়ে যায় না, আজীবন থাকে।
- B: ইউজার ট্যাবটি বন্ধ করলে।
- C: ইউজার ব্রাউজারটিকে পুরোপুরি বন্ধ করলে, কেবলমাত্র ট্যাব না।
- D: ইউজার তার কম্পিউটার বন্ধ করলে।

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

`sessionStorage` এ সংরক্ষিত ডেটা ট্যাব বন্ধ করার পরে মুছে যায়।

যদি আপনি `localStorage` ব্যবহার করতেন, তবে ডেটা সাধারণত আজীবন থাকতো, যদি এক্ষেত্রে `localStorage.clear()` ব্যবহার না করা হয়।

</p>
</details>

---

###### ২৩. আউটপুট কি হবে?

```javascript
var num = 8;
var num = 10;

console.log(num);
```

- A: `8`
- B: `10`
- C: `SyntaxError`
- D: `ReferenceError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

`var` কীওয়ার্ড ব্যবহার করে আপনি একই নামে একাধিক ভেরিয়েবল ডিক্লেয়ার করতে পারবেন। সেক্ষেত্রে ভেরিয়েবলটি সর্বশেষ মানটিকে ধারণ করবে।

কিন্তু `let` বা `const` দিয়ে এটা করা সম্ভব নয় কারণ এগুলি ব্লক-স্কোপড হয়ে থাকে।

</p>
</details>

---

###### ২৪. আউটপুট কি হবে?

```javascript
const obj = { 1: 'a', 2: 'b', 3: 'c' };
const set = new Set([1, 2, 3, 4, 5]);

obj.hasOwnProperty('1');
obj.hasOwnProperty(1);
set.has('1');
set.has(1);
```

- A: `false` `true` `false` `true`
- B: `false` `true` `true` `true`
- C: `true` `true` `false` `true`
- D: `true` `true` `true` `true`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

আপনি যদি অবজেক্টের কীগুলোকে স্ট্রিং আকারে নাও লিখেন তবুও এটি ভিতরে ভিতরে স্ট্রিং-এ রূপান্তরিত হয়ে থাকে (সিম্বল বাদে)। এই কারনে `obj.hasOwnProperty('1')` এটি `true` রিটার্ন করে।

কিন্তু সেটের জন্য এটি এভাবে কাজ করে না। আমাদের সেটে কোনো `'1'` কী (key) নেই: এজন্য `set.has('1')` এটি `false` রিটার্ন করে। এটার নাম্বার টাইপের `1` কী (key) আছে, এজন্য `set.has(1)` এটি `true` রিটার্ন করে।

</p>
</details>

---

###### ২৫. আউটপুট কি হবে?

```javascript
const obj = { a: 'one', b: 'two', a: 'three' };
console.log(obj);
```

- A: `{ a: "one", b: "two" }`
- B: `{ b: "two", a: "three" }`
- C: `{ a: "three", b: "two" }`
- D: `SyntaxError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

যদি আপনার একই নামে দুইটি কী (key) থাকে, তবে প্রথম কী (key) টি পরিবর্তিত হবে। এটি তখনো তার প্রথম অবস্থানে থাকবে, কিন্তু সর্বশেষ মানটি ধারণ করবে।

</p>
</details>

---

###### ২৬. জাভাস্ক্রিপ্টের গ্লোবাল এক্সিকিউশন কনটেক্স্ট আপনার জন্য দুটি জিনিস তৈরি করে দেয়: গ্লোবাল অবজেক্ট এবং "this" কীওয়ার্ড।

- A: সত্য
- B: মিথ্যা
- C: এটা বিষয়টি নির্ভর করে

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

বেস এক্সিকিউশন কনটেক্স্টটি হলো গ্লোবাল এক্সিকিউশন কনটেক্স্ট: এটি আপনার কোডের সর্বত্র এক্সেস করা যায়।

</p>
</details>

---

###### ২৭. আউটপুট কি হবে?

```javascript
for (let i = 1; i < 5; i++) {
  if (i === 3) continue;
  console.log(i);
}
```

- A: `1` `2`
- B: `1` `2` `3`
- C: `1` `2` `4`
- D: `1` `3` `4`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

`continue` স্টেটমেন্টটি একটি নির্দিষ্ট শর্ত যদি `true` হয়, তবে একটি ইটারেশন স্কীপ করে যায়।

</p>
</details>

---

###### ২৮. আউটপুট কি হবে?

```javascript
String.prototype.giveLydiaPizza = () => {
  return 'Just give Lydia pizza already!';
};

const name = 'Lydia';

console.log(name.giveLydiaPizza())
```

- A: `"Just give Lydia pizza already!"`
- B: `TypeError: not a function`
- C: `SyntaxError`
- D: `undefined`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

`String` হলো একটি বিল্ট-ইন কন্সট্রাক্টর যেটাতে আমরা প্রপার্টি যোগ করতে পারি। আমি শুধুমাত্র এটার প্রোটোটাইপে একটা মেথড যোগ করেছি। প্রিমিটিভ স্ট্রিংগুলি স্বয়ংক্রিয়ভাবে স্ট্রিং অবজেক্টে রূপান্তরিত হয়, যা স্ট্রিং প্রোটোটাইপ ফাংশন দ্বারা তৈরি করা হয়। তাই, সব স্ট্রিং (স্ট্রিং অবজেক্টগুলি) ঐ মেথডটি অ্যাক্সেস করতে পারে।

</p>
</details>

---

###### ২৯. আউটপুট কি হবে?

```javascript
const a = {};
const b = { key: 'b' };
const c = { key: 'c' };

a[b] = 123;
a[c] = 456;

console.log(a[b]);
```

- A: `123`
- B: `456`
- C: `undefined`
- D: `ReferenceError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

অবজেক্টের কীগুলি স্বয়ংক্রিয়ভাবে স্ট্রিং হিসাবে রূপান্তরিত হয়। আমরা অবজেক্ট `a`-তে একটি অবজেক্টকে কী (key) হিসাবে সেট করার চেষ্টা করছি, যার মান `123`। 

তবে, আমরা যখন একটি অবজেক্টকে স্ট্রিং-এ রূপান্তরিত করি, তখন এটি `"[object Object]"` হয়ে যায়। তাই আমরা এখানে বলছি, `a["[object Object]"] = 123`। এরপর আমরা একই কাজটি আবার করতে পারি। `c` অন্য আরেকটি অবজেক্ট যা আমরা শর্টকাট ভাবে স্ট্রিং-এ রূপান্তরিত করেছি। সুতরাং `a["[object Object]"] = 456`।

এরপর আমরা `a[b]`-কে লগ করেছি যা মূলত: `a["[object Object]"]` এটা। আমরা কিছুটা আগেই সেটার ভ্যালু হিসেবে `456` সেট করেছি, তাই এটি `456` রিটার্ন করে।

</p>
</details>

---

###### ৩০. আউটপুট কি হবে?

```javascript
const foo = () => console.log('First');
const bar = () => setTimeout(() => console.log('Second'));
const baz = () => console.log('Third');

bar();
foo();
baz();
```

- A: `First` `Second` `Third`
- B: `First` `Third` `Second`
- C: `Second` `First` `Third`
- D: `Second` `Third` `First`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

আমাদের কাছে একটা `setTimeout` ফাংশন আছে এবং আমরা এটাকে প্রথমেই কল করেছি, তবে এটি শেষে লগ হয়েছে।

এর কারণ, আমাদের ব্রাউজারগুলিতে শুধুমাত্র রানটাইম ইঞ্জিনটি নয়, `WebAPI` নামে আরো একটি জিনিস আছে। `WebAPI` শুরুতেই আমাদেরকে `setTimeout` ফাংশনটি সরবরাহ করে, যেমন ডম।

কলব্যাক ফাংশনটি `WebAPI`-তে পুশ করার পরেও `setTimeout` ফাংশনটি নিজেই স্ট্যাক থেকে পপ হয়ে যায় (তবে কলব্যাকটি নয়!)।

<img src="https://i.imgur.com/X5wsHOg.png" width="200">

এখন `foo` ফাংশনটি কল হয়েছে এবং `"First"` লগ হচ্ছে।

<img src="https://i.imgur.com/Pvc0dGq.png" width="200">

`foo` ফাংশনটি স্ট্যাক থেকে পপ হয়ে গেছে এবং `baz` ফাংশনটি কল করা হয়েছে। `"Third"` লগ হয়েছে।

<img src="https://i.imgur.com/WhA2bCP.png" width="200">

`WebAPI` চাইলেই যখন তখন স্ট্যাকে যে কোনকিছু যোগ করতে পারে না। এটি এর পরিবর্তে কিউ (queue) নামক একটা জিনিসে কলব্যাক ফাংশনটিকে পুশ করে।

<img src="https://i.imgur.com/NSnDZmU.png" width="200">

এখানে একটি **ইভেন্ট লুপ** কাজ করা শুরু করে। ইভেন্ট লুপ স্ট্যাক এবং টাস্ক কিউ পর্যবেক্ষণ করে। যদি স্ট্যাক খালি থাকে, তবে এটি কিউ-এর প্রথম জিনিসটি নিয়ে এটি স্ট্যাকে পুশ করে।

<img src="https://i.imgur.com/uyiScAI.png" width="200">

`bar` ফাংশনটি কল হয়েছে, `"Second"` লগ হয়েছে এবং এটা স্ট্যাক থেকে পপ হয়েছে।

</p>
</details>

---

###### ৩১. বাটনে ক্লিক করলে `event.target` কোন হবে?

```html
<div onclick="console.log('first div')">
  <div onclick="console.log('second div')">
    <button onclick="console.log('button')">
      Click!
    </button>
  </div>
</div>
```

- A: বাইরের `div`
- B: ভিতরের `div`
- C: `button` নিজেই
- D: সমস্ত নেস্টেড উপাদানগুলির একটি অ্যারে।

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

সবচেয়ে গভীরতম নেস্টেড উপাদানটি ইভেন্ট সৃষ্টি করেছে, এটিই ইভেন্টের টার্গেট। আপনি `event.stopPropagation`-এর দ্বারা ইভেন্ট বাবলিং বন্ধ করতে পারবেন।

</p>
</details>

---

###### ৩২. আপনি প্যারাগ্রাফটিতে ক্লিক করলে লগের আউটপুট কি হবে?

```html
<div onclick="console.log('div')">
  <p onclick="console.log('p')">
    Click here!
  </p>
</div>
```

- A: `p` `div`
- B: `div` `p`
- C: `p`
- D: `div`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

আমরা যখন `p` এলিমেন্টে ক্লিক করি, তখন আমরা দুটি লগ দেখতে পাই: `p` এবং `div`। ইভেন্ট প্রোপাগেশনের তিনটি ধাপ আছে: ক্যাপচারিং, টার্গেট এবং বাবলিং। ডিফল্ট অবস্থায় ইভেন্ট হ্যান্ডলারগুলি বাবলিং ফেজে কার্যকর হয় (যদি না আপনি `useCapture` কে `true` সেট করেন)। এটি সবচেয়ে ভিতরের নেস্টেড উপাদান থেকে বাইরের দিকে যায়।

</p>
</details>

---

###### ৩৩. আউটপুট কি হবে?

```javascript
const person = { name: 'Lydia' };

function sayHi(age) {
  return `${this.name} is ${age}`;
}

console.log(sayHi.call(person, 21));
console.log(sayHi.bind(person, 21));
```

- A: `undefined is 21` `Lydia is 21`
- B: `function` `function`
- C: `Lydia is 21` `Lydia is 21`
- D: `Lydia is 21` `function`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

উভয়ের দ্বারা `this` কীওয়ার্ডটি কোন অবজেক্টেকে রেফার করবে সেটা সেট করে দিতে পারি। যাইহোক, `.call` ফাংশনটিও সাথে সাথে এক্সিকিউট হয়!

`.bind`-এর ক্ষেত্রে এমনটি হয়না, এটি ফাংশনটির একটি কপি রিটার্ন করে, তবে সেটা একটা কন্টেক্সটের ভিতরে! এটি সাথে সাথে এক্সিকিউট হয় না।

</p>
</details>

---

###### ৩৪. আউটপুট কি হবে?

```javascript
function sayHi() {
  return (() => 0)();
}

console.log(typeof sayHi());
```

- A: `"object"`
- B: `"number"`
- C: `"function"`
- D: `"undefined"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

IIFE (Immediately Invoked Function Expression) ফাংশনটি যে মান রিটার্ন করে, `sayHi` ফাংশনটি সেই রিটার্নকৃত মানটি রিটার্ন করে। এই ফাংশনটি `0` রিটার্ন করে, যা `"number"` টাইপের।

আপনার জানার জন্য: `typeof` নিম্নলিখিত মানগুলি রিটার্ন করতে পারে: `undefined`, `boolean`, `number`, `bigint`, `string`, `symbol`, `function` এবং `object`। মনে রাখবেন যে `typeof null` `"object"` রিটার্ন করে।

</p>
</details>

---

###### ৩৫. এই মানগুলির মধ্যে কোনটি কোনটি মিথ্যা (falsy)?

```javascript
0;
new Number(0);
('');
(' ');
new Boolean(false);
undefined;
```

- A: `0`, `''`, `undefined`
- B: `0`, `new Number(0)`, `''`, `new Boolean(false)`, `undefined`
- C: `0`, `''`, `new Boolean(false)`, `undefined`
- D: সবগুলোই মিথ্যা

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

জাভাস্ক্রিপ্টে আটটি মিথ্যা (falsy) মান রয়েছে:

- `undefined`
- `null`
- `NaN`
- `false`
- `''` (খালি স্ট্রিং)
- `0`
- `-0`
- `0n` (BigInt(0))

ফাংশন কন্সট্রাক্টর, যেমন `new Number` এবং `new Boolean` এগুলো মিথ্যা (falsy) নয়, বরং সত্য (truthy)।

</p>
</details>

---

###### ৩৬. আউটপুট কি হবে?

```javascript
console.log(typeof typeof 1);
```

- A: `"number"`
- B: `"string"`
- C: `"object"`
- D: `"undefined"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

`typeof 1` স্টেটমেন্টটি `"number"` রিটার্ন করে। যেহেতু এটি একটি স্ট্রিং সেহেতু
`typeof "number"` স্টেটমেন্টটি `"string"` রিটার্ন করে।

</p>
</details>

---

###### ৩৭. আউটপুট কি হবে?

```javascript
const numbers = [1, 2, 3];
numbers[10] = 11;
console.log(numbers);
```

- A: `[1, 2, 3, null x 7, 11]`
- B: `[1, 2, 3, 11]`
- C: `[1, 2, 3, empty x 7, 11]`
- D: `SyntaxError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

যখন আপনি একটি অ্যারের কোনো এলিমেন্টে ভ্যালু সেট করেন যা অ্যারের দৈর্ঘ্যকে অতিক্রম করে, তখন জাভাস্ক্রিপ্ট কিছু "ফাঁকা স্লট" তৈরী করে। এই ফাঁকা স্লট গুলোতে আসলে `undefined` ভ্যালু থাকে, কিন্তু আপনি কিছুটা নীচের মতো করে দেখতে পাবেন:

`[1, 2, 3, empty x 7, 11]`

আপনি এটিকে কোথায় রান করছেন তার উপর নির্ভর করে (এটি ব্রাউজার, নোড ইত্যাদি অনুসারে পরিবর্তিত হতে পারে)। 

</p>
</details>

---

###### ৩৮. আউটপুট কি হবে?

```javascript
(() => {
  let x, y;
  try {
    throw new Error();
  } catch (x) {
    (x = 1), (y = 2);
    console.log(x);
  }
  console.log(x);
  console.log(y);
})();
```

- A: `1` `undefined` `2`
- B: `undefined` `undefined` `undefined`
- C: `1` `1` `2`
- D: `1` `undefined` `undefined`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

`catch` ব্লকটি `x` আর্গুমেন্টটি পায়, এই আর্গুমেন্ট এবং ফাংশনের ভিতরে ডিক্লেয়ার করা ভেরিয়েবল `x` একই নয়। `catch`-এর ভিতরে এই `x` ভেরিয়েবলটি ব্লক স্কোপড।

পরবর্তীতে, আমরা এই ব্লক-স্কোপড ভেরিয়েবলকে `1` এর সমান সেট করেছি এবং ভেরিয়েবল `y` এর মানকে সেট করেছি। এখন আমরা ব্লক-স্কোপড ভেরিয়েবল `x` কে লগ করেছি যা `1` এর সমান।

`catch` ব্লকের বাইরে `x` এখনও `undefined` থেকে গেছে এবং `y` হলো `2`। `catch` ব্লকের বাইরে `console.log(x)` করলে `undefined` রিটার্ন হয় এবং `y` রিটার্ন হয় `2`।

</p>
</details>

---

###### ৩৯. জাভাস্ক্রীপ্টে সবকিছুই হয় একটি...

- A: প্রিমিটিভ অথবা অবজেক্ট
- B: ফাংশন অথবা অবজেক্ট
- C: ট্রিকি প্রশ্ন! শুধুই অবজেক্ট
- D: নাম্বার অথবা অবজেক্ট

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

জাভাস্ক্রিপ্টে শুধুমাত্র প্রিমিটিভ এবং অবজেক্ট টাইপ রয়েছে।

প্রিমিটিভ টাইপ গুলো হলো `boolean`, `null`, `undefined`, `bigint`, `number`, `string`, এবং `symbol`।

অবজেক্টের সাথে প্রিমিটিভের পার্থক্য হলো প্রিমিটিভের কোনো প্রোপার্টি বা মেথড নেই; তবে, আপনি দেখতে পাবেন যে, `'foo'.toUpperCase()` এক্সপ্রেশনটি `TypeError` দেয়নি, বরং এটি `'FOO'` রিটার্ন করে। এটার কারণ, আপনি যখন স্ট্রিং এর মতো প্রিমিটিভ টাইপের উপর প্রপার্টি বা মেথড অ্যাক্সেস করার চেষ্টা করেন, তখন জাভাস্ক্রিপ্ট ইমপ্লিসিটভাবে প্রিমিটিভ টাইপটিতে একটি রেপার ক্লাস, যেমন `String`, দ্বারা আবৃত করে এবং এক্সপ্রেশন এক্সিকিউট হওয়ার পর তা তাত্ক্ষণিকভাবে মুছে ফেলে। `null` এবং `undefined` ছাড়া অন্যান্য সকল প্রিমিটিভগুলো এধরণের আচরণ প্রদর্শন করে।

</p>
</details>

---

###### ৪০. আউটপুট কি হবে?

```javascript
[[0, 1], [2, 3]].reduce(
  (acc, cur) => {
    return acc.concat(cur);
  },
  [1, 2],
);
```

- A: `[0, 1, 2, 3, 1, 2]`
- B: `[6, 1, 2]`
- C: `[1, 2, 0, 1, 2, 3]`
- D: `[1, 2, 6]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

`[1, 2]` আমাদের প্রথম বা ইনিশিয়াল মান। এই মানটাকে নিয়েই আমরা শুরু করি এবং এটিই প্রথম `acc` এর মান। প্রথম রাউন্ডে, `acc` হলো `[1,2]` এবং `cur` হলো `[0, 1]`। আমরা তাদেরকে যুক্ত করি যার ফলাফল হিসাবে পাওয়া যায় `[1, 2, 0, 1]`।

তারপর, `acc` হলো `[1, 2, 0, 1]` এবং `cur` হলো `[2, 3]`। আমরা তাদেরকে যুক্ত করি যার ফলাফল হিসাবে পাওয়া যায় `[1, 2, 0, 1, 2, 3]`।

</p>
</details>

---

###### ৪১. আউটপুট কি হবে?

```javascript
!!null;
!!'';
!!1;
```

- A: `false` `true` `false`
- B: `false` `false` `true`
- C: `false` `true` `true`
- D: `true` `true` `false`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

`null` হলো মিথ্যা। `!null` মানে হচ্ছে `true`। `!true` মানে হচ্ছে `false`।

`""` হলো মিথ্যা। `!""` মানে হচ্ছে `true`। `!true` মানে হচ্ছে `false`।

`1` হলো সত্য। `!1` মানে হচ্ছে `false`। `!false` মানে হচ্ছে `true`।

</p>
</details>

---

###### ৪২. ব্রাউজারে `setInterval` মেথডটি কি রিটার্ন করে?

```javascript
setInterval(() => console.log('Hi'), 1000);
```

- A: একটা ইউনিক আইডি
- B: নির্দিষ্ট মিলিসেকেন্ডের পরিমাণ
- C: পাঠানো ফাংশনটি
- D: `undefined`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

এটি একটি ইউনিক আইডি রিটার্ন করে। এই আইডিটি ব্যবহার করে `clearInterval()` ফাংশন দিয়ে ঐ ইন্টারভালটি বাতিল করা যেতে পারে।

</p>
</details>

---

###### ৪৩. এটা কি রিটার্ন করে?

```javascript
[...'Lydia'];
```

- A: `["L", "y", "d", "i", "a"]`
- B: `["Lydia"]`
- C: `[[], "Lydia"]`
- D: `[["L", "y", "d", "i", "a"]]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

একটি স্ট্রিং-কে ইটারেট করা যায়। স্প্রেড (spread) অপারেটর প্রতিটি অক্ষরকে ইটারেট করে একটি এলিমেন্ট আকারে ম্যাপ করে।

</p>
</details>

---

###### ৪৪. আউটপুট কি হবে?

```javascript
function* generator(i) {
  yield i;
  yield i * 2;
}

const gen = generator(10);

console.log(gen.next().value);
console.log(gen.next().value);
```

- A: `[0, 10], [10, 20]`
- B: `20, 20`
- C: `10, 20`
- D: `0, 10 and 10, 20`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

সাধারণ ফাংশনগুলি কল করার পর মাঝ-পথে থেমে থাকতে পারে না। তবে, একটি জেনারেটর ফাংশন মাঝ-পথে থেমে থাকতে পারে এবং পরবর্তীতে যেখানে থেমেছিলো সেখান থেকে কন্টিনিউ করতে পারে। প্রতিবার জেনারেটর ফাংশনটি `yield` কীওয়ার্ড দ্বারা বাঁধা প্রাপ্ত হয় এবং সেই কীওয়ার্ডের পরে উল্লিখিত মানটি রিটার্ন করে। মনে রাখবেন, এক্ষেত্রে জেনারেটর ফাংশনটি ঐ মানটি রিটার্ন করে না, বরং মানটি তৈরী করে।

প্রথমে আমরা `i` এর মান হিসাবে `10` সেট করে জেনারেটর ফাংশনটি ইনিশিয়ালাইজ করেছি। আমরা `next()` মেথড ব্যবহার করে জেনারেটর ফাংশনটি কল করছি। জেনারেটর ফাংশনটি প্রথমবার কল করলে, `i` হচ্ছে `10`। সে প্রথম `yield` কীওয়ার্ড সংগ্রহ করে: এটি `i` এর মান তৈরী করে। জেনারেটরটি এখন স্থগিত হয়ে গেছে, এবং `10` প্রিন্ট হয়েছে।

তারপর, আমরা আবার `next()` মেথড ব্যবহার করে ফাংশনটি কল করলাম। এটি আগে যে জায়গা থেকে থেমে গিয়েছিলো সেই জায়গা থেকে কন্টিনিউ করবে, এখনো `i` এর মান `10` এর সমান। এখন, এটি পরবর্তী `yield` কীওয়ার্ড পাইলে, এটি `i * 2` বসিয়ে দিবে। `i` এর মান `10` এর সমান, সুতরাং এটি `10 * 2` রিটার্ন করবে অর্থাৎ `20` রিটার্ন করবে। এর ফলে `10, 20` পাওয়া যায়।

</p>
</details>

---

###### ৪৫. এটা কি রিটার্ন করে?

```javascript
const firstPromise = new Promise((res, rej) => {
  setTimeout(res, 500, 'one');
});

const secondPromise = new Promise((res, rej) => {
  setTimeout(res, 100, 'two');
});

Promise.race([firstPromise, secondPromise]).then(res => console.log(res));
```

- A: `"one"`
- B: `"two"`
- C: `"two" "one"`
- D: `"one" "two"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

যখন আমরা `Promise.race` মেথডে একাধিক প্রমিস পাঠাই, তখন এটি প্রথম যে প্রমিসটি রিসলভ (resolve)/রিজেক্ট (reject) হয় সে অনুযায়ী রিসলভ/রিজেক্ট করে। আমরা প্রথম প্রমিসের (`firstPromise`) জন্য `setTimeout` মেথডে ৫০০ মিলিসেকেন্ড এবং দ্বিতীয় প্রমিসের (`secondPromise`) জন্য ১০০ মিলিসেকেন্ড টাইমার পাঠিয়েছি। এর মানে হলো `secondPromise`-টি প্রথমে রিসলভ হয় এবং এর মান হলো `'two'`। `res` এখন `'two'` ধারণ করে আছে যা পরবর্তীতে লগ হচ্ছে।

</p>
</details>

---

###### ৪৬. আউটপুট কি হবে?

```javascript
let person = { name: 'Lydia' };
const members = [person];
person = null;

console.log(members);
```

- A: `null`
- B: `[null]`
- C: `[{}]`
- D: `[{ name: "Lydia" }]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

প্রথমে আমরা `person` নামে একটি ভেরিয়েবল ডিক্লেয়ার করেছি যেটা একটি অবজেক্ট হিসেবে আছে এবং সেটির `name` নামে একটি প্রোপার্টি আছে।

<img src="https://i.imgur.com/TML1MbS.png" width="200">

তারপরে, `members` নামে আমরা আরও একটি ভেরিয়েবল (অ্যারে) ডিক্লেয়ার করেছি। আমরা অ্যারের প্রথম উপাদান হিসেবে `person`-কে সেট করেছি। যখন অবজেক্টগুলি একে অপরের সমান করা হয় তখন তারা রেফারেন্সের মাধ্যমে ইন্টারএক্ট করে। যখন আপনি একটি ভেরিয়েবলের সাথে অন্য ভেরিয়েবলকে রেফারেন্সের দ্বারা অ্যাসাইন করেন তখন আসলে আপনি ঐ রেফরেন্সের কপি তৈরি করেন। (মনে রাখবেন যে তারা আসলে একই রেফারেন্সকে পয়েন্ট করে নাই!)।

<img src="https://i.imgur.com/FSG5K3F.png" width="300">

তারপরে, আমরা `person` ভেরিয়েবলকে `null`-এর সমান করি।

<img src="https://i.imgur.com/sYjcsMT.png" width="300">

আমরা শুধুমাত্র `person` ভেরিয়েবলের মান পরিবর্তন করছি এবং অ্যারের প্রথম উপাদানটি পরিবর্তন করছি না, কারণ ঐ উপাদানটিতে অবজেক্টের অন্য একটি (কপি) রেফারেন্স আছে। `members` এর প্রথম উপাদানটি এখনো মূল অবজেক্টের রেফারেন্স ধারণ করে আছে। আমরা `members` অ্যারেটি লগ করলে, প্রথম উপাদানটি এখনো অবজেক্টের মানটি ধারণ করে আছে যা লগ হচ্ছে।

</p>
</details>

---

###### ৪৭. আউটপুট কি হবে?

```javascript
const person = {
  name: 'Lydia',
  age: 21,
};

for (const item in person) {
  console.log(item);
}
```

- A: `{ name: "Lydia" }, { age: 21 }`
- B: `"name", "age"`
- C: `"Lydia", 21`
- D: `["name", "Lydia"], ["age", 21]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

একটি `for-in` লুপ দ্বারা আমরা অবজেক্টের কীগুলির উপর ইটারেট করতে পারি, যেমন এক্ষেত্রে `name` এবং `age`। অবজেক্টের কীগুলি মূলত স্ট্রিং (সিম্বল না হলে)। প্রতিটি লুপে আমরা `item` ভেরিয়েবলের মানকে বর্তমান ইটারেশনের কী (key)-এর সমান করে দেই। প্রথমে, `item` হলো `name` এবং এটি লগ করা হচ্ছে। তারপরে, `item` হলো `age` যা পরবর্তীতে লগ হচ্ছে।

</p>
</details>

---

###### ৪৮. আউটপুট কি হবে?

```javascript
console.log(3 + 4 + '5');
```

- A: `"345"`
- B: `"75"`
- C: `12`
- D: `"12"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

অপারেটর অ্যাসোসিয়েটিভিটি হলো কম্পাইলার কিভাবে এক্সপ্রেশনগুলি মূল্যায়ন করবে সেটা, সাধারণত বাম থেকে ডানে বা ডান থেকে বামে। এটি শুধুমাত্র তখনই ঘটে যখন সমস্ত অপারেটরের অগ্রাধিকার বা প্রিসিডেন্স একই থাকে। আমাদের শুধুমাত্র এক ধরনের অপারেটর আছে: `+`। যোগের ক্ষেত্রে অ্যাসোসিয়েটিভিটি বামে থেকে ডানে হয়।

প্রথমে `3 + 4` ইভালুয়েট হয়। এটার ফলাফল হয় `7`।

কোয়ারসনের কারণে `7 + '5'` এক্সিকিউট করলে তার ফলাফল হয় `"75"`। জাভাস্ক্রিপ্ট সংখ্যা `7` কে স্ট্রিং-এ রূপান্তর করে, প্রশ্ন ১৫ দেখুন। আমরা দুটি স্ট্রিং কে `+` অপারেটর ব্যবহার করে যোগ করতে পারি। `"7" + "5"` এর ফলাফল `"75"`।

</p>
</details>

---

###### ৪৯. `num`-এর মান কোনটি?

```javascript
const num = parseInt('7*6', 10);
```

- A: `42`
- B: `"42"`
- C: `7`
- D: `NaN`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

স্ট্রিংটিতে শুধুমাত্র প্রথম সংখ্যাটি রিটার্ন করেছে। রেডিক্স (দ্বিতীয় আর্গুমেন্ট) অনুসারে (কোন ধরণের সংখ্যা পার্স করতে চাইছি: দশমিক, হেক্সাডেসিমাল, অক্টাল, বাইনারি ইত্যাদি) `parseInt` মেথডটি স্ট্রিংয়ের ক্যারেক্টারগুলি ভ্যালিড বা বৈধ সংখ্যা কিনা তা পরীক্ষা করে। রেডিক্স অনুসারে যখন কোনো ইন-ভ্যালিড বা অবৈধ ক্যারেক্টার পায় তখন এটি পার্সিং বন্ধ করে দেয় এবং পরবর্তী ক্যারেক্টারগুলি ইগনোর করে।

`*` একটি বৈধ সংখ্যা নয় তাই এটি শুধুমাত্র `"7"` কে দশমিক সংখ্যা `7` এ পার্স করে। `num` এখন `7` মানটি ধারণ করে আছে।

</p>
</details>

---

###### ৫০. আউটপুট কি হবে?

```javascript
[1, 2, 3].map(num => {
  if (typeof num === 'number') return;
  return num * 2;
});
```

- A: `[]`
- B: `[null, null, null]`
- C: `[undefined, undefined, undefined]`
- D: `[ 3 x empty ]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

অ্যারের ম্যাপিং এর সময়, `num` ভেরিয়েবলের মান হলো লুপে চলমান বর্তমান উপাদানটি। এক্ষেত্রে উপাদানগুলি হলো সংখ্যা, সুতরাং if স্টেটমেন্টির `typeof num === "number"` কন্ডিশনটি সত্য হয়। ম্যাপ ফাংশনটি একটি নতুন অ্যারে তৈরি করে এবং ফাংশন থেকে ফেরত পাওয়া মানগুলি ঐ অ্যারেতে সন্নিবেশ করে রিটার্ন করে।

তবে, আমরা কোনো মান রিটার্ন করিনি। যখন আমরা ফাংশন থেকে কোন মান রিটার্ন না করি তখন ফাংশনটি `undefined` রিটার্ন করে। প্রতিটি উপাদানের জন্য ফাংশন ব্লকটি কল হয়, তাই প্রতিটি উপাদানের জন্য আমরা `undefined` রিটার্ন করছি।

</p>
</details>

---

###### ৫১. আউটপুট কি হবে?

```javascript
function getInfo(member, year) {
  member.name = 'Lydia';
  year = '1998';
}

const person = { name: 'Sarah' };
const birthYear = '1997';

getInfo(person, birthYear);

console.log(person, birthYear);
```

- A: `{ name: "Lydia" }, "1997"`
- B: `{ name: "Sarah" }, "1998"`
- C: `{ name: "Lydia" }, "1998"`
- D: `{ name: "Sarah" }, "1997"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

আর্গুমেন্ট যদি অবজেক্ট না হয় তাহলে তার _মান_ পাস করা হয় (call by value), তবে অবজেক্টের ক্ষেত্রে তাদের _রেফারেন্স_ পাস করা হয় (call by reference)। `birthYear` একটি স্ট্রিং হওয়ায় এটির মান পাস করা হয়। মান দ্বারা আর্গুমেন্ট পাস করলে, ঐ মানটির একটি _কপি_ তৈরি হয় (৪৬ নাম্বার প্রশ্নটি দেখুন)।

ভেরিয়েবল `birthYear` এর `"1997"` মানের জন্য একটি রেফারেন্স রয়েছে। আর্গুমেন্ট `year` এর ও `"1997"` মানের জন্য একটি রেফারেন্স রয়েছে, কিন্তু এই রেফারেন্সটি এবং `birthYear` এর রেফারেন্সটি একই নয়। আমরা যখন `"1998"` দ্বারা `year` মানটি আপডেট করছি তখন আমরা শুধুমাত্র `year` মানটি আপডেট করছি, `birthYear` এর মান এখনো `"1997"` আছে।

`person` ভেরিয়েবলটির মান একটি অবজেক্ট। আর্গুমেন্ট `member` এর একটি (কপি) রেফারেন্স রয়েছে ঐ একই অবজেক্টের। আমরা যখন `member` অবজেক্টের একটি প্রপার্টি পরিবর্তন করি তখন `person` এর মানও একই ভাবে পরিবর্তিত হবে, কারণ তারা উভয়ে একই অবজেক্টকে রেফারেন্স করে রয়েছে। একারণে `person` এর `name` প্রপার্টিটির মান এখন `"Lydia"`।

</p>
</details>

---

###### ৫২. আউটপুট কি হবে?

```javascript
function greeting() {
  throw 'Hello world!';
}

function sayHi() {
  try {
    const data = greeting();
    console.log('It worked!', data);
  } catch (e) {
    console.log('Oh no an error:', e);
  }
}

sayHi();
```

- A: `It worked! Hello world!`
- B: `Oh no an error: undefined`
- C: `SyntaxError: can only throw Error objects`
- D: `Oh no an error: Hello world!`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

`throw` স্টেটমেন্ট ব্যবহার করে আমরা কাস্টম এরর তৈরি করতে পারি। এই স্টেটমেন্ট ব্যবহার করে আপনি এক্সেপশন থ্রো করতে পারেন। এক্সেপশন হতে পারে একটি <b>স্ট্রিং</b>, একটি <b>নাম্বার</b>, একটি <b>বুলিয়ান</b> বা একটি <b>অবজেক্ট</b>। এই ক্ষেত্রে, আমাদের এক্সেপশন হলো স্ট্রিং `'Hello world!'`.

`catch` স্টেটমেন্ট ব্যবহার করে আমরা নির্দিষ্ট করে বলতে পারি যে যখন ট্রাই ব্লকে একটি এক্সেপশন থ্রো হয় তখন কি করবেন। এখানে স্ট্রিং ব্যবহার করে একটি এক্সেপশন থ্রো করা হয়েছে: `'Hello world!'`। `e` এখন সেই স্ট্রিং এর সমান, যেটা আমরা লগ করছি। এর ফলাফল হলো `'Oh an error: Hello world!'`।

</p>
</details>

---

###### ৫৩. আউটপুট কি হবে?

```javascript
function Car() {
  this.make = 'Lamborghini';
  return { make: 'Maserati' };
}

const myCar = new Car();
console.log(myCar.make);
```

- A: `"Lamborghini"`
- B: `"Maserati"`
- C: `ReferenceError`
- D: `TypeError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

যখন আপনি একটি প্রপার্টি রিটার্ন করেন তখন প্রপার্টির মানটি রিটার্ন করা মানের সমান হয়, কনস্ট্রাক্টর ফাংশনে সেট করা মানের সমান হয় না। আমরা স্ট্রিং `"Maserati"` রিটার্ন করেছি, তাই `myCar.make` এর মান `"Maserati"` এর সমান হয়।

</p>
</details>

---

###### ৫৪. আউটপুট কি হবে?

```javascript
(() => {
  let x = (y = 10);
})();

console.log(typeof x);
console.log(typeof y);
```

- A: `"undefined", "number"`
- B: `"number", "number"`
- C: `"object", "number"`
- D: `"number", "undefined"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

`let x = (y = 10);` এটা আসলে নিচের কোডের শর্টহ্যান্ড নোটেশন:

```javascript
y = 10;
let x = y;
```

যখন আমরা `y` কে `10` এর সমান সেট করি তখন আসলে আমরা গ্লোবাল অবজেক্টে (`window` ব্রাউজারে এবং `global` নোডে) একটি প্রপার্টি `y` যুক্ত করেছি। একটি ব্রাউজারে, `window.y` এখন `10` এর সমান।

এরপর আমরা `x` নামক একটি ভেরিয়েবলে `y` কে এ্যাসাইন করেছি যার মান `10`। `let` কীওয়ার্ড ব্যবহার করে ডিক্লেয়ার করা ভেরিয়েবলগুলি ব্লক স্কোপ হয়, এগুলো যে ব্লকের ভিতরে ডিক্লেয়ার করা হয় শুধুমাত্র সেই ব্লকের মধ্যে ডিফাইন করা হয়; এক্ষেত্রে ইমিডিয়েটলি ইনভোক্ড ফাংশন এক্সপ্রেশন (IIFE) এর মধ্যে সেটা করা হয়েছে। আমরা যখন `typeof` অপারেটর ব্যবহার করছি তখন সেই ব্লকে অপারেন্ড `x` ডিক্লেয়ার করা নাই: আমরা ডিক্লেয়ার করা ব্লকের বাইরে থেকে `x` কে অ্যাক্সেস করার চেষ্টা করছি। এর মানে `x` ডিফাইন করা নাই, আনডিফাইন্ড। যে ভ্যালুর কোনো মান প্রদান করা হয়নি বা ডিক্লেয়ার করা হয়নি তাদের টাইপ হলো `"undefined"`। এই কারণে `console.log(typeof x)` রেজাল্ট হিসেবে `"undefined"` রিটার্ন করে।

তবে, আমরা যখন `y` কে `10` এর সমান সেট করেছি তখন একটি গ্লোবাল ভেরিয়েবল ‌`y` তৈরি করেছি। এই মানটি আমাদের কোডে যেকোনো জায়গা থেকে অ্যাক্সেস করা যায়। `y` কে ডিফাইন করা হয়েছে এবং এটি `"number"` টাইপের মান ধারণ করে আছে। এজন্য `console.log(typeof y)` রেজাল্ট হিসেবে `"number"` রিটার্ন করে।

</p>
</details>

---

###### ৫৫. আউটপুট কি হবে?

```javascript
class Dog {
  constructor(name) {
    this.name = name;
  }
}

Dog.prototype.bark = function() {
  console.log(`Woof I am ${this.name}`);
};

const pet = new Dog('Mara');

pet.bark();

delete Dog.prototype.bark;

pet.bark();
```

- A: `"Woof I am Mara"`, `TypeError`
- B: `"Woof I am Mara"`, `"Woof I am Mara"`
- C: `"Woof I am Mara"`, `undefined`
- D: `TypeError`, `TypeError`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

আমরা `delete` কীওয়ার্ড ব্যবহার করে অবজেক্টের প্রপার্টিগুলি ডিলেট করতে পারি, এটি প্রোটোটাইপের উপরও প্রয়োগ করা যায়। প্রোটোটাইপে একটি প্রপার্টি ডিলেট করার পর এটি আর প্রোটোটাইপ চেইনে পাওয়া যায় না। এক্ষেত্রে `delete Dog.prototype.bark` এর পরে প্রোটোটাইপে `bark` ফাংশনটি আর পাওয়া যায় না, যদিও আমরা এখনো এটিকে অ্যাক্সেস করার চেষ্টা করছি।

যখন আমরা আসলে এমন কিছু কল করার চেষ্টা করছি যেটি আসলে কোনো ফাংশন না তখন একটি `TypeError` থ্রো হয়। এক্ষেত্রে `TypeError: pet.bark is not a function` হয়, কারণ `pet.bark` হলো `undefined`।

</p>
</details>

---

###### ৫৬. আউটপুট কি হবে?

```javascript
const set = new Set([1, 1, 2, 3, 4]);

console.log(set);
```

- A: `[1, 1, 2, 3, 4]`
- B: `[1, 2, 3, 4]`
- C: `{1, 1, 2, 3, 4}`
- D: `{1, 2, 3, 4}`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: D

`Set` অবজেক্টটি হলো ইউনিক মানগুলির একটা কালেকশান: সেটে একটি মান কেবলমাত্র একবারই পাওয়া যাবে।

আমরা একটি ডুপ্লিকেট মান `1` সহ ইটারেবল `[1, 1, 2, 3, 4]` পাস করেছি। যেহেতু সেটে আমরা একই মান দুইবার থাকতে পারে না, সেহেতু তাদের মধ্যে একটি মুছে ফেলা হয়। একারণে ফলাফল স্বরূপ `{1, 2, 3, 4}` পাওয়া যায়।

</p>
</details>

---

###### ৫৭. আউটপুট কি হবে?

```javascript
// counter.js
let counter = 10;
export default counter;
```

```javascript
// index.js
import myCounter from './counter';

myCounter += 1;

console.log(myCounter);
```

- A: `10`
- B: `11`
- C: `Error`
- D: `NaN`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

একটি ইম্পোর্ট করা মডিউল _রিড-ওনলি_ হয়: অর্থাৎ আপনি ইম্পোর্ট করা মডিউলটি পরিবর্তন করতে পারবেন না। এই মডিউলগুলো যেখান থেকে এক্সপোর্ট করা হয়েছে শুধুমাত্র সেখান থেকে এই মান পরিবর্তন করতে পারে।

আমরা `myCounter` এর মানকে বাড়ানোর চেষ্টা করলে এটি একটি এরর থ্রো করে: `myCounter` টি রিড-ওনলি এবং এটাকে পরিবর্তন করা যাবে না।

</p>
</details>

---

###### ৫৮. আউটপুট কি হবে?

```javascript
const name = 'Tajnur';
age = 21;

console.log(delete name);
console.log(delete age);
```

- A: `false`, `true`
- B: `"Tajnur"`, `21`
- C: `true`, `true`
- D: `undefined`, `undefined`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

`delete` অপারেটরটি একটি বুলিয়ান মান রিটার্ন করে: সফলভাবে ডিলিট করে ফেললে `true` রিটার্ন করে, অন্যথায় `false` রিটার্ন করে। তবে `var`, `const` বা `let` কীওয়ার্ড দিয়ে ডিক্লেয়ার করা ভেরিয়েবলগুলি `delete` অপারেটর ব্যবহার করে ডিলিট করা যায় না।

`name` ভেরিয়েবলটি `const` কীওয়ার্ড ব্যবহার করে ডিক্লেয়ার করা হয়েছিল, সুতরাং এটি ডিলিট করার কাজটি সফল হয়নি: এজন্য এটি `false` রিটার্ন করে। `age` ভেরিয়েবলে `21` সেট করায় আমরা আসলে গ্লোবাল অবজেক্টে `age` নামক একটি প্রপার্টি যুক্ত করেছি। আপনি চাইলে এভাবে কোনো অবজেক্টের এমনকি গ্লোবাল অবজেক্টেরও প্রোপার্টি সফলভাবে ডিলিট করতে পারবেন, সুতরাং `delete age` সফলভাবে `true` রিটার্ন করে।

</p>
</details>

---

###### ৫৯. আউটপুট কি হবে?

```javascript
const numbers = [1, 2, 3, 4, 5];
const [y] = numbers;

console.log(y);
```

- A: `[[1, 2, 3, 4, 5]]`
- B: `[1, 2, 3, 4, 5]`
- C: `1`
- D: `[1]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: C

আমরা অ্যারে থেকে অ্যারের মানগুলি অথবা অবজেক্ট থেকে অবজেক্টের প্রপার্টিগুলি ডিস্ট্রাকচারিং এর মাধ্যমে বের করে আনতে পারি। উদাহরণস্বরূপ:

```javascript
[a, b] = [1, 2];
```

<img src="https://i.imgur.com/ADFpVop.png" width="200">

`a` এর মান এখন `1` এবং `b` এর মান এখন `2`। আমরা আসলে প্রশ্নে যেটা করেছি তা হলো:

```javascript
[y] = [1, 2, 3, 4, 5];
```

<img src="https://i.imgur.com/NzGkMNk.png" width="200">

এটার মানে হলো `y` এর মান অ্যারের প্রথম মানের সমান, যেটা সংখ্যা `1`। আমরা `y` লগ করলে `1` রিটার্ন হয়।

</p>
</details>

---

###### ৬০. আউটপুট কি হবে?

```javascript
const user = { name: 'Tajnur', age: 28 };
const admin = { admin: true, ...user };

console.log(admin);
```

- A: `{ admin: true, user: { name: "Tajnur", age: 28 } }`
- B: `{ admin: true, name: "Tajnur", age: 28 }`
- C: `{ admin: true, user: ["Tajnur", 28] }`
- D: `{ admin: true }`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

স্প্রেড অপারেটর `...` ব্যবহার করে অবজেক্টকে কম্বাইন বা সংযোজন করা সম্ভব। এটি আপনাকে একটি অবজেক্টের প্রোপার্টিগুলো কী/ভ্যালু পেয়ার বা জোড়া আকারে কপি তৈরি করতে দেয় এবং সেগুলোকে অন্য একটি অবজেক্টে যোগ করতে দেয়। এক্ষেত্রে আমরা `user` অবজেক্টের একটি কপি তৈরি করে তা `admin` অবজেক্টে যোগ করেছি। `admin` অবজেক্টটি এখন কপি করে নেওয়া কী/ভ্যালু পেয়ার গুলো ধারণ করে আছে, যা ফলাফল হিসেবে `{ admin: true, name: "Tajnur", age: 28 }` পাওয়া যায়।

</p>
</details>

---

###### ৬১. আউটপুট কি হবে?

```javascript
const person = { name: 'Lydia' };

Object.defineProperty(person, 'age', { value: 21 });

console.log(person);
console.log(Object.keys(person));
```

- A: `{ name: "Lydia", age: 21 }`, `["name", "age"]`
- B: `{ name: "Lydia", age: 21 }`, `["name"]`
- C: `{ name: "Lydia"}`, `["name", "age"]`
- D: `{ name: "Lydia"}`, `["age"]`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: B

`defineProperty` মেথড ব্যবহার করে আমরা একটি অবজেক্টে নতুন প্রপার্টি যোগ করতে পারি বা বিদ্যমান প্রপার্টিগুলি পরিবর্তন করতে পারি। `defineProperty` মেথড ব্যবহার করে একটি প্রপার্টি যখন অবজেক্টে যোগ করা হয়, তখন ডিফল্টভাবে সেগুলি _not enumerable_ অবস্থায় থাকে অর্থাৎ অপ্রকাশ্য থাকে। `Object.keys` মেথডটি অবজেক্ট থেকে সব _প্রকাশ্য_ প্রপার্টির নাম রিটার্ন করে, এই ক্ষেত্রে শুধুমাত্র `"name"` রিটার্ন করেছে।

`defineProperty` মেথড ব্যবহার করে যোগ করা প্রপার্টিগুলি ডিফল্টভাবে অপরিবর্তনীয়। আপনি `writable`, `configurable` এবং `enumerable` প্রপার্টিগুলি ব্যবহার করে এই আচরণটি ওভাররাইড করতে পারবেন। এভাবে `defineProperty` মেথড আপনাকে অবজেক্টে যে প্রপার্টিগুলি যোগ করছেন তার উপর আরো বেশি নিয়ন্ত্রণ দেয়।

</p>
</details>

---

###### ৬২. আউটপুট কি হবে?

```javascript
const settings = {
  username: 'lydiahallie',
  level: 19,
  health: 90,
};

const data = JSON.stringify(settings, ['level', 'health']);
console.log(data);
```

- A: `"{"level":19, "health":90}"`
- B: `"{"username": "lydiahallie"}"`
- C: `"["level", "health"]"`
- D: `"{"username": "lydiahallie", "level":19, "health":90}"`

<details><summary><b>উত্তর</b></summary>
<p>

#### উত্তর: A

`JSON.stringify` এর দ্বিতীয় আর্গুমেন্টটি হলো _রিপ্লেসার_। রিপ্লেসারটি একটি ফাংশন অথবা অ্যারে হতে পারে এবং মানগুলি কি এবং কিভাবে স্ট্রিংগিফাই করা হবে সেটা নির্দিষ্ট করে দিতে আপনাকে এটার উপর আরো নিয়ন্ত্রন দেয়।

যদি রিপ্লেসারটি একটি _অ্যারে_ হয়, তবে কেবলমাত্র অ্যারেতে থাকা প্রোপার্টির নামগুলি স্ট্রিং-এ যোগ করা হবে। এক্ষেত্রে `"level"` এবং `"health"` নামের প্রোপার্টিগুলি শুধুমাত্র অন্তর্ভুক্ত করা হয়েছে, `"username"` প্রোপার্টি বাদ দেয়া হয়। `data` এখন `"{"level":19, "health":90}"` এটার সমান।

যদি রিপ্লেসারটি একটি _ফাংশন_ হয়, তবে এই ফাংশনটি স্ট্রিংগিফাই করা অবজেক্টের প্রতিটি প্রোপার্টিতে কল হয়। এই ফাংশন থেকে রিটার্ন করা প্রতিটি প্রোপার্টির মান জেসন স্ট্রিং-এ যোগ করা হবে। যদি মানটি `undefined` হয়, তবে এই প্রোপার্টিটি জেসন স্ট্রিং থেকে বাদ দেয়া হবে।

</p>
</details>

---

###### ৬৩. আউটপুট কি হবে?

```javascript
let num = 10;

const increaseNumber = () => num++;
const increasePassedNumber = number => number++;

const num1 = increaseNumber();
const num2 = increasePassedNumber(num1);

console.log(num1);
console.log(num2);
```

- A: `10`, `10`
- B: `10`, `11`
- C: `11`, `11`
- D: `11`, `12`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: A

The unary operator `++` _first returns_ the value of the operand, _then increments_ the value of the operand. The value of `num1` is `10`, since the `increaseNumber` function first returns the value of `num`, which is `10`, and only increments the value of `num` afterwards.

`num2` is `10`, since we passed `num1` to the `increasePassedNumber`. `number` is equal to `10`(the value of `num1`. Again, the unary operator `++` _first returns_ the value of the operand, _then increments_ the value of the operand. The value of `number` is `10`, so `num2` is equal to `10`.

</p>
</details>

---

###### 64. What's the output?

```javascript
const value = { number: 10 };

const multiply = (x = { ...value }) => {
  console.log((x.number *= 2));
};

multiply();
multiply();
multiply(value);
multiply(value);
```

- A: `20`, `40`, `80`, `160`
- B: `20`, `40`, `20`, `40`
- C: `20`, `20`, `20`, `40`
- D: `NaN`, `NaN`, `20`, `40`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: C

In ES6, we can initialize parameters with a default value. The value of the parameter will be the default value, if no other value has been passed to the function, or if the value of the parameter is `"undefined"`. In this case, we spread the properties of the `value` object into a new object, so `x` has the default value of `{ number: 10 }`.

The default argument is evaluated at _call time_! Every time we call the function, a _new_ object is created. We invoke the `multiply` function the first two times without passing a value: `x` has the default value of `{ number: 10 }`. We then log the multiplied value of that number, which is `20`.

The third time we invoke multiply, we do pass an argument: the object called `value`. The `*=` operator is actually shorthand for `x.number = x.number * 2`: we modify the value of `x.number`, and log the multiplied value `20`.

The fourth time, we pass the `value` object again. `x.number` was previously modified to `20`, so `x.number *= 2` logs `40`.

</p>
</details>

---

###### 65. What's the output?

```javascript
[1, 2, 3, 4].reduce((x, y) => console.log(x, y));
```

- A: `1` `2` and `3` `3` and `6` `4`
- B: `1` `2` and `2` `3` and `3` `4`
- C: `1` `undefined` and `2` `undefined` and `3` `undefined` and `4` `undefined`
- D: `1` `2` and `undefined` `3` and `undefined` `4`

<details><summary><b>Answer</b></summary>
<p>

#### Answer: D

The first argument that the `reduce` method receives is the _accumulator_, `x` in this case. The second argument is the _current value_, `y`. With the reduce method, we execute a callback function on every element in the array, which could ultimately result in one single value.

In this example, we are not returning any values, we are simply logging the values of the accumulator and the current value.

The value of the accumulator is equal to the previously returned value of the callback function. If you don't pass the optional `initialValue` argument to the `reduce` method, the accumulator is equal to the first element on the first call.

On the first call, the accumulator (`x`) is `1`, and the current value (`y`) is `2`. We don't return from the callback function, we log the accumulator and current value: `1` and `2` get logged.

If you don't return a value from a function, it returns `undefined`. On the next call, the accumulator is `undefined`, and the current value is `3`. `undefined` and `3` get logged.

On the fourth call, we again don't return from the callback function. The accumulator is again `undefined`, and the current value is `4`. `undefined` and `4` get logged.

</p>
</details>
  
---
