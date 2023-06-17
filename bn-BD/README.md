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

`catch` ব্লকটি `x` আর্গুমেন্টটি পায়, এই আর্গুমেন্ট এবং ফাংশনের ভিতরে ডিক্লেয়ার করা ভ্যারিয়েবল `x` একই নয়। `catch`-এর ভিতরে এই `x` ভ্যারিয়েবলটি ব্লক স্কোপড।

পরবর্তীতে, আমরা এই ব্লক-স্কোপড ভ্যারিয়েবলকে `1` এর সমান সেট করেছি এবং ভ্যারিয়েবল `y` এর মানকে সেট করেছি। এখন আমরা ব্লক-স্কোপড ভ্যারিয়েবল `x` কে লগ করেছি যা `1` এর সমান।

`catch` ব্লকের বাইরে `x` এখনও `undefined` থেকে গেছে এবং `y` হলো `2`। `catch` ব্লকের বাইরে `console.log(x)` করলে `undefined` রিটার্ন হয় এবং `y` রিটার্ন হয় `2`।

</p>
</details>

---
