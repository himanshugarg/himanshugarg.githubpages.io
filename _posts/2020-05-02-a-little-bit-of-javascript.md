---
layout: default
categories: javascript
---

## कैलकुलेटर

कंप्यूटर जी पर ब्राउज़र खोलें, Ctrl Shift K एक साथ दबाएं, और गणित का कोई सवाल टाईप करें:-
```javascript
>> 9*9*9;
729
```
कंप्यूटर जी आपके सवाल का हल निकाल कर आपको देंगे। यह काम एक साधारण कैलकुलेटर पर भी हो जाएगा। या शायद आप अपने मन में ही इसे हल कर लें।

---
* 1 का 0 से भाग देकर देखें क्या आता है? 
```javascript
>> 1/0;
```

---


## नाम देना
कंप्यूटर जी को आप और भी बहुत से काम बता सकते हैं। आप कंप्यूटर जी को कह सकते हैं कि दिये गये नाम की एक जगह बनाएं और वहां हल को संभाल कर रख लें।
```javascript
let cube9 = 729;
```
जिससे जरूरत पड़ने पर आप हल याद करने के बजाय उसका नाम उपयोग कर सकें।
```javascript
>> cube9;
729
```

किसी नये हल को नये नाम की जगह बना कर वहां रख सकते हैं।
```javascript
>> let cube10 = 1000;
>> cube10;
1000
```

और बाद में उन हलों को लिखने के बजाय उनके नामों से ही नये सवालों का हल निकाल सकते हैं
```javascript
>> cube9 + cube10;
1729

```

---
* यदि हमें किसी नई संख्या जैसे कि 12 के साथ सवाल का हल निकालना हो तो फिर 12 * 12 * 12 लिखना होगा। क्या ऐसा हो सकता है कि हम कंप्यूटर जी को सवाल का हल निकालने का तरीका ही याद करा दें? (किसी संख्या को खुद से तीन बार गुणा करने से उस संख्या का घन निकलता है, जैसे 10 का घन 1000 है)

---

कंप्यूटर जी पर हम अपना काम और भी कम कर सकते हैं। हम उन्हें कह सकते हैं कि दिये गये नाम की एक जगह बनाएं जहां हल निकालने के तरीके को ही संभाल कर रख लें:- 
```javascript
>> let cube = function (n) {
	return n*n*n;
}
```

ऐसा करने से हमने एक function बना दिया है। अब वह काम करने के लिये बस उस काम का नाम ही काफी है, क्योंकि हमने कंप्यूटर जी को उस नाम का मतलब याद करा दिया है। अब हमारे पास कुछ वैसी ही मशीन बन गई है जिसमें जो सिक्का डालेंगे उसी के अनुसार वो आपका काम करेगी। अब हम अन्य सवालों का हल करा सकते हैं जिनमें वही तरीका काम आता है। 
```javascript
>> cube(9);
729
>> cube(10);
1000
>> cube(9) + cube(10);
1729
>> cube(8) + cube(11);
1842
```
---

* क्या और कोई संख्याऐं हैं जिन्हें cube(?) + cube(?) करने पर 1729 आता हो? कुछ अलग-अलग संख्याओं के साथ आज़माएं यदि 1729 आ जाये।
```javascript
>> cube(7) + cube(12)
```

* sumCubes नाम की एक जगह बनाएं जो दी गई दो संख्याओं को खुद से तीन बार गुणा करके जोड़ कर बताए।
```javascript
let sumCubes = function(a, b) {
?
}
>> sumCubes(2, 3) 
35
```

---
## जांच करना
यदि हमें कंप्यूटर जी से कुछ ढूंढने का काम कराना हो तो कंप्यूटर जी के पास यह पता करने का तरीका होना चाहिये कि वह चीज़ उन्हें मिल गई। कंप्यूटर जी के पास ऐसा तरीका है बस आपको उन्हें बताना होगा जांच क्या करनी है:-
```javascript
>> if (cube(12) + cube(1) == 1729) {
	console.log('sum of 12 cubed and 1 cubed is 1729');
} 
```

और जांच के सफल या असफल होने पर अलग-अलग काम कर सकते हैं:-
```javascript
if (cube(13) + cube(0) != 1729) {
	console.log('13 cubed is not 1729');
} else {
	console.log('13 cubed is 1729');
}
```

---

* checkSumOfCubes नाम की एक जगह बनाएं जो दी गई दो संख्याओं के खुद से गुणा कर जोड़ कर देखे कि 1729 आता है या नहीं।
```javascript
>> let checkSumOfCubes = function(a, b) {
>> if (cube(a) + cube(b) == 1729) {
		return ?;
	} else {
		return ?;
	}
}
>> checkSumOfCubes(1, 11)
true
>> checkSumOfCubes(2, 10)
false
```

---

## दोहराना
किसी काम को बार-बार कराने के लिये हम उस काम को बार-बार लिख सकते हैं। 
```javascript
>> console.log('जय हो!');
जय हो!
>> console.log('जय हो!');
जय हो!
>> console.log('जय हो!');
जय हो!
```

या कंप्यूटर जी को बता सकते हैं कि इस एक काम को हमेशा करते रहें।

```javascript
>> while (true) {
	console.log('जय हो!');
}
```

पर कंप्यूटर जी अगर हमेशा एक ही काम करते रहे तो हम उनसे और कोई काम नहीं करा पायेंगे। हो सकता है कि उन्हें रोकना भी मुश्किल हो जाए।

---
* इसको चला कर देखें क्या होता है।

```javascript
>> let n = 0;

>> n = n+1;
>> console.log(n);

>> n = n+1;
>> console.log(n)

...
```

* पिछले सवाल में जो काम बार-बार हो रहा है उसे while से कैसे कराएंगे
```javascript
let n = 0;
while (true) {
	?
}
```
* इस सवाल में जो काम बार-बार हो रहा है उसे while से कैसे कराएंगे।

```javascript
>> let n = 0;
>> let product = 1;

>> n = n+1;
>> product = product * 10;
>> console.log(n);

>> n = n+1;
>> product = product * 10
>> console.log(n)
```

---

किसी काम को हमेशा करते रहने कि बजाय हम कंप्यूटर जी को हम बता सकते हैं कि काम को दोहराने से पहले जांच कर लें कि काम को आगे करना भी है या नहीं।
```javascript
>> let n = 0;
>> while (n < 10) {
	console.log(n);
	n = n+1;
}
```

---
* यदि हमें किसी संख्या को खुद से ही 100 बार गुणा करना हो तो कैसे करेंगे? 

---

## सूची बनाना
यदि हमें एक जैसा काम कई चीज़ों पर दोहराना हो तो उन सबको नए नाम देने होंगे। इससे अच्छा होगा कि हम उन चीज़ों की एक सूची बना कर कंप्यूटर जी को उसे संभाल कर रखने के लिये कहें:-
```javascript
>> let greetings = ['सलाम', 'नमस्ते', 'हैलो'];
>> let fib = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89];
```

अब हम कंप्यूटर जो को सूची की पहली चीज़ पर कुछ करने के लिये कह सकते हैं।
```javascript
>> console.log(names[0]);
सलाम
```

सूची की दूसरी चीज़ पर कुछ करने के लिये कह सकते हैं।
```javascript
>> console.log(names[1]);
सलाम
```

सूची में कितनी चीज़ें हैं पता कर सकते हैं।
```javascript
>> console.log(names.length);
3
```

सूची की आखरी चीज़ पर कुछ करने के लिये कह सकते हं।
```javascript
console.log(names[names.length-1]);
हैलो
```

---
* यदि हमें 1 से 100 तक की संख्याओं की सूची बनानी हो तो कैसे बनाएंगे?
* numbersUpto नाम की एक जगह बनाएं जो 1 से लेकर दी गई संख्या तक की संख्याओं की एक सूची बना कर दे।
```
>> let range = function(start, end) {
	let numbers = [];
	while (start <= end) {
		?
	}	
}
>> console.log(numbersUpto(10));
```

---

हम सूची में नई चीज जोड़ सकते हैं:-
```javascript
>> greetings.push('सत् स्री अकाल');
>> greetings.push('सत् स्री अकाल');
>> console.log(names.length);
5
>> console.log(names[3]);
सत् स्री अकाल
>> console.log(names[4]);
सत् स्री अकाल
```

सूची की सारी चीज़ों पर कुछ बताया गया काम करा सकते हैं:-
```javascript
>> greetings.forEach(function(item, index, array) {
	console.log(item, index);
});
```

---
*  इसको चला कर देखें क्या आता है
```javascript
>> greetings.forEach(function(item1, index1, array1) {
	greetings.forEach(function(item2, index2, array2) {
		console.log(item1, item2);
	});
});
```

*  पिछले सवाल में कुछ लाईनें आती हैं जिनकी शायद हमें जरूरत ना हो, यदि हमें उनको हटाना हो तो क्या कर सकते हं:-
```javascript
>> greetings.forEach(function(item1, index1, array1) {
	greetings.forEach(function(item2, index2, array2) {
		if (item1 < item2) {
			console.log(item1, item2);
		}
	});
});
```

---

सूची में पता लगा सकते हैं कि कोई चीज़ कहां पर है:-
```javascript
>> console.log(greetings.indexOf('सलाम'));
0
>> console.log(greetings.indexOf('अलविदा'));
-1
```
---
* 1 से 11 तक की संख्याओं को खुद से तीन बार गुणा करके एक सूची बनाएं।
```javascript
	let list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
	let listOfCubes = [];
	list.forEach(function(item, index, array) {
		listOfCubes.push(?);
	});
```
*  getListOfCubes नाम की एक जगह बनाएं जो दी गई संख्या तक की सारी संख्याओं के घनों की एक सूची बना कर दे
```javascript
>> let getListOfCubes = function(n) {
	?
}
>> let list = getListOfCubes(11);
>> console.log(list[list.length-1]);
1729
```

---

यह एक function है जो हमें 9999 तक की सभी ऐसी संख्याएं बता देता है जो 2 संख्याओं के घनों से बनती हैं। 
```javascript
let taxiNos = function() {
	let list = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 
		    12, 13, 14, 15, 16, 17, 18, 19, 20, 21];
	let nos = [];
	list.forEach(function(item1, index1, array1) {
		list.forEach(function(item2, index2, array2) {
			let sum = item1*item1*item1 + item2*item2*item2;
			// यदि sum चार अंकों तक का ही है और अभी तक नहीं मिला है
			if (sum <= 9999 && nos.indexOf(sum) == -1) {
				nos.push(sum);
			}
		}
	}
	return nos;
}
```
कुछ असाधारण लोग इतनी गणित तो बिना कंप्यूटर जी के ही कर लेते हैं। 

## और जानने के लिये
* स्ट्रक्चर एंड इंटरप्रेटेशन ऑफ कंप्यूटर प्रोग्राम्स - <https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html>
* जावास्क्रिप्ट एम डी एन - <https://developer.mozilla.org/en-US/docs/Web/JavaScript>
* Taxicab number - <https://en.wikipedia.org/wiki/Taxicab_number>
* खान एकेडमी फ्री ऑनलाईन कोर्स, पाठ और अभ्यास - <https://www.khanacademy.org>
* LeetCode - दुनिया का अग्रणी ऑनलाईन प्रोग्रामिंग सीखने का प्लैटफॉर्म - <https://www.leetcode.com>
