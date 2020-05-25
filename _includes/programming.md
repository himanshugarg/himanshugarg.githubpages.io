![Srinivasa Ramanujan](/assets/RamanujanCambridge.jpg)  चार्ल्स एफ. विल्सन द्वारा खींची इस फोटो में श्रीनिवास रामानुजन बीच में और उनके गुरू जी. एच. हार्डी तस्वीर में दायीं ओर हैं।

बात 1919 की है जब श्रीनिवास रामानुजन लंदन में थे। उनके मित्र और गुरू, जी. एच. हार्डी उनसे मिलने एक टैक्सी से गये। उस टैक्सी का नंबर था 1729। बातचीत में उन्होंने रामानुजन को बताया, "मेरी टैक्सी का नंबर बड़ा साधारण था। यह किसी बुरे वक्त का संकेत तो नहीं"। "नहीं बिल्कुल नहीं", रामानुजन बोले, "यह कोई साधारण संख्या नहीं। यह सबसे छोटी संख्या है, जो बनती है दो संख्याओं के घनों को जोड़कर, दो अलग-अलग तरीकों से।"


{% case page.lang %}
	{% when "ruby" %}
आइये, हम भी कंप्यूटर जी के साथ रूबी में बात करते-करते ऐसी ही मजेदार संख्याएं ढूंढें।
कंप्यूटर जी पर `Terminal` या `Command Prompt` खोलें, `irb` टाइप करें, और फिर गणित का कोई सवाल टाईप करें।
	{% when "python" %}
आइये, हम भी कंप्यूटर जी के साथ पाइथॉन में बात करते-करते ऐसी ही मजेदार संख्याएं ढूंढें।
कंप्यूटर जी पर `Terminal` या `Command Prompt` खोलें, `python` टाइप करें, और फिर गणित का कोई सवाल टाईप करें।
	{% else %}
आइये, हम भी कंप्यूटर जी के साथ जावास्क्रिप्ट में बात करते-करते ऐसी ही मजेदार संख्याएं ढूंढें।
कंप्यूटर जी पर फायरफॉक्स ब्राउज़र खोलें, Ctrl Shift K एक साथ दबाएं, और गणित का कोई सवाल टाईप करें। 
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
> 9 * 9 * 9
=> 729

> 10 * 10 * 10
=> 1000

> 9 * 9 * 9 + 10 * 10 * 10
=> 1729

```
  {% when "python" %}
```python
>>> 9 * 9 * 9
729

>>> 10 * 10 * 10
1000

>>> 9 * 9 * 9 + 10 * 10 * 10
1729
```
  {% else %}
```javascript
>> 9 * 9 * 9;
729

>> 10 * 10 * 10;
1000

>> 9 * 9 * 9 + 10 * 10 * 10;
1729

```
{% endcase %}

कंप्यूटर जी के साथ हम अपनी खोज और भी आसान कर सकते हैं। हम संख्याओं को नाम दे सकते हैं और फिर उन संख्याओं को याद रखने के बजाय उनका नाम ही ले सकते हैं।

{% case page.lang %}
{% when "ruby" %}
```ruby
> cube9 = 729
=> 729

> cube10 = 1000
=> 1000

> cube9 + cube10 
=> 1729

> cube10 - cube9
=> 271

```
  {% when "python" %}
```python
>>> cube9 = 729
>>> cube9
729
>>> cube10 = 1000
>>> cube10
1000
>>> cube9 + cube10
1729
>>> cube10 - cube9
271
```
  {% else %}
```javascript
>> let cube9 = 729;
>> cube9;
729
>> let cube10 = 1000;
>> cube10;
1000
>> cube9 + cube10;
1729
>> cube10 - cube9
271
```
{% endcase %}

हम संख्याओं को नाम देने के साथ-साथ उन्हें बनाने के तरीके को भी नाम दे सकते हैं। और फिर कंप्यूटर जी को काम का पूरा तरीका बार-बार बताने के बजाय, बस तरीके का नाम ही ले सकते हैं।
 
{% case page.lang %}
  {% when "ruby" %}
```ruby
> def cube(n) 
>     return n * n * n
> end
=> :cube
> cube(9)
=> 729

> cube(10)
=> 1000

> cube(9) + cube(10)
=> 1729

> cube(8) + cube(11)
=> 1843

> cube(cube(10))
=> 1000000
```
{% when "python" %}
```python
>>> def cube(n): 
...     return n * n * n
>>> cube(9)
729
>>> cube(10)
1000
>>> cube(9) + cube(10)
1729
>>> cube(8) + cube(11)
1843
>>> cube(cube(10))
1000000
```
  {% else %}
```javascript
>> let cube = function (n) {
    return n * n * n;
}
>> cube(9);
729
>> cube(10);
1000
>> cube(9) + cube(10);
1729
>> cube(8) + cube(11);
1843
>> cube(cube(10))
1000000
```
{% endcase %}




* क्या और कोई संख्याऐं हैं जिन्हें cube(?) + cube(?) करने पर 1729 आता हो? कुछ अलग-अलग संख्याओं के साथ आज़माएं यदि 1729 आ जाये? {% case page.lang %}
{% when "ruby" %}
```ruby
> cube(7) + cube(12)
```
{% when "python" %}
```python
>>> cube(7) + cube(12)
```
  {% else %}
```javascript
>> cube(7) + cube(12)
```
{% endcase %}

* दो संख्याओं को खुद से तीन बार गुणा करके जोड़ने का तरीका लिखें और उसको sumCubes नाम दें। {% case page.lang %}
{% when "ruby" %}
```ruby
def sumCubes(a, b)
	?
end
> sumCubes(2, 3)
=> 35
```
{% when "python" %}
```python
def sumCubes (a, b):
...    ?
>>> sumCubes(2, 3) 
35
```
  {% else %}
```javascript
let sumCubes = function(a, b) {
?
}
>> sumCubes(2, 3) 
35
```
{% endcase %}


कोई नई संख्या मिलने पर वो खास है कि नहीं यह पता करने का काम अभी हमें ही करना पड़ रहा है। इसके बजाय हम कंप्यूटर जी को बता सकते हैं कि कैसे पता करें कि कोई संख्या खास है कि नहीं। जिससे वो खुद पता लगा कर अलग-अलग स्थिति में अलग-अलग काम कर सकें।
 
{% case page.lang %}
  {% when "ruby" %}
```ruby
> if cube(12) + cube(1) == 1729
>     puts("sum of 12 cubed and 1 cubed is 1729")
=> nil

> if cube(13) + cube(0) != 1729
>     puts("13 cubed is not 1729")
> else
>     puts("13 cubed is 1729")
13 cubed is not 1729
=> nil
```
{% when "python" %}
```python
>>> if cube(12) + cube(1) == 1729: 
...     print('sum of 12 cubed and 1 cubed is 1729')
>>> if cube(13) + cube(0) != 1729:
...     print('13 cubed is not 1729')
... else:
...     print('13 cubed is 1729')

```
{% else %}
```javascript
>> if (cube(12) + cube(1) == 1729) {
    console.log('sum of 12 cubed and 1 cubed is 1729');
} 
>> if (cube(13) + cube(0) != 1729) {
    console.log('13 cubed is not 1729');
} else {
    console.log('13 cubed is 1729');
}
```
{% endcase %}



* checkSumOfCubes नाम की एक दी गई दो संख्याओं के खुद से गुणा कर जोड़ कर देखे कि 1729 आता है या नहीं। {% case page.lang %}
{% when "ruby" %}
```ruby
>>> def checkSumOfCubes(a, b)
...     if cube(a) + cube(b) == 1729
...         true
...     else
...         false
>>> checkSumOfCubes(1, 11)
true
>>> checkSumOfCubes(2, 10)
false
```
{% when "python" %}
```python
>>> def checkSumOfCubes(a, b):
...     if cube(a) + cube(b) == 1729:
...         return ?
...     else:
...         return ?
>>> checkSumOfCubes(1, 11)
true
>>> checkSumOfCubes(2, 10)
false
```
  {% else %}
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
{% endcase %}


किसी काम को बार-बार कराने के लिये हम उस काम को बार-बार बता सकते हैं। 
 
{% case page.lang %}
  {% when "ruby" %}
```ruby
> puts("जय हो!")
जय हो!
=> nil

> puts("जय हो!")
जय हो!
=> nil

> puts("जय हो!")
जय हो!
=> nil
```
{% when "python" %}
```python
>>> print('जय हो!')
जय हो!
>>> print('जय हो!')
जय हो!
>>> print('जय हो!')
जय हो!

```
  {% else %}
```javascript
>> console.log('जय हो!');
जय हो!
>> console.log('जय हो!');
जय हो!
>> console.log('जय हो!');
जय हो!
```
{% endcase %} 
या कंप्यूटर जी को कह सकते हैं कि उस एक काम को बार-बार करते रहें।
{% case page.lang %}
  {% when "ruby" %}
```ruby
> while true
>     puts("जय हो")
> end
```
{% when "python" %}
```python
>>> while (true):
...     print('जय हो!')
```
  {% else %}

```javascript
>> while (true) {
    console.log('जय हो!');
}
```
{% endcase %}

* इसको चला कर देखें क्या होता है। {% case page.lang %}

  {% when "ruby" %}
```ruby
>>> n = 0
>>> n = n+1
>>> puts(n)
>>> n = n+1
>>> puts(n)
```
{% when "python" %}
```python
>>> n = 0
>>> n = n+1
>>> print(n)
>>> n = n+1
>>> print(n)
...
```
{% else %}
```javascript
>> let n = 0;
>> n = n+1;
>> console.log(n);
>> n = n+1;
>> console.log(n)
...

```
{% endcase %}

* पिछले सवाल में जो काम बार-बार हो रहा है उसे while से कैसे कराएंगे? {% case page.lang %}
  {% when "python" %}
```ruby
> n = 0
> while (true)
>   ?
> end
```
```python
>>> n = 0
>>> while (true):
...    ?
```
  {% else %}
```javascript
>> let n = 0;
>> while (true) {
    ?
}
```
{% endcase %}

* इस सवाल में जो काम बार-बार हो रहा है उसे while से कैसे कराएंगे? {% case page.lang %}
  {% when "ruby" %}
```ruby
> n = 0
> product = 1
> n = n+1
> product = product * 10
> puts(n)
10
> n = n+1
> product = product * 10
> puts(n)
100
```
{% when "python" %}
```python
>>> n = 0
>>> product = 1

>>> n = n+1
>>> product = product * 10
>>> print(n)

>>> n = n+1
>>> product = product * 10
>>> print(n)
```
  {% else %}
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
{% endcase %}



किसी काम को हमेशा के लिये करते रहने के बजाय हम कंप्यूटर जी को कह सकते हैं कि काम को दोहराने से पहले जांच कर लें कि काम को आगे करना भी है या नहीं।


{% case page.lang %}
  {% when "ruby" %}
  ```ruby
> n = 0
> while n < 10
>     puts n
>     n = n+1
> end
0
1
2
3
4
5
6
7
8
9
=> nil
```

  {% when "python" %}
```python
>>> n = 0
>>> while n < 10:
...    print(n)
...    n = n+1
```

{% else %}
```javascript
>> let n = 0;
>> while (n < 10) {
    console.log(n);
    n = n+1;
}
```
{% endcase %}



* यदि हमें किसी संख्या को खुद से ही 100 बार गुणा करना हो तो कैसे करेंगे? 


एक जैसी बहुत सारी चीज़ों पर कुछ काम करना हो तो सबके अलग-अलग नाम रखने के बजाय हम उन चीज़ों की एक सूची बना सकते हैं।
o
{% case page.lang %}
	{% when "ruby" %}
```ruby
> greetings = ["सलाम", "नमस्ते", "हैलो"]
=> ["सलाम", "नमस्ते", "हैलो"]

> fib = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
=> [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```
    {% when "python" %}
```python
>>> greetings = ['सलाम', 'नमस्ते', 'हैलो']
>>> fib = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]
```
  {% else %}
```javascript
>> let greetings = ['सलाम', 'नमस्ते', 'हैलो'];
>> let fib = [1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89];
```
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
>>> puts(names[0])
सलाम
=> nil
```
  {% when "python" %}
```python
>>> print(names[0])
सलाम
```
  {% else %}
```javascript
>> console.log(names[0]);
सलाम
```
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
> puts(names[1])
नमस्ते
=> nil
```
  {% when "python" %}
```python
>>> print(names[1])
नमस्ते
```
  {% else %}
```javascript
>> console.log(names[1]);
नमस्ते
```
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
> puts(names.length)
3
=> nil
```
  {% when "python" %}
```python
>>> print(len(names))
3
```
  {% else %}
```javascript
>> console.log(names.length);
3
```
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
puts(names[names.length - 1])
हैलो
```
  {% when "python" %}
```python
print(names[len(names) - 1])
हैलो
```
  {% else %}
```javascript
console.log(names[names.length-1]);
हैलो
```

{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
> greetings.push('सत् श्री अकाल')
> greetings.push('सत् श्री अकाल')
> puts(len(greetings));
5
> puts(greetings[3]);
सत् श्री अकाल
> puts(greetings[4]);
सत् श्री अकाल
```
  {% when "python" %}
```python
>>> greetings.push('सत् श्री अकाल')
>>> greetings.push('सत् श्री अकाल')
>>> print(len(greetings));
5
>>> print(greetings[3]);
सत् श्री अकाल
>>> print(greetings[4]);
सत् श्री अकाल
```
  {% else %}
```javascript
>> greetings.push('सत् श्री अकाल');
>> greetings.push('सत् श्री अकाल');
>> console.log(greetings.length);
5
>> console.log(greetings[3]);
सत् श्री अकाल
>> console.log(greetings[4]);
सत् श्री अकाल
```
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
greetings.each { |item| puts(item) }
```
  {% when "python" %}
```python
>>> for item in greetings:
...     print(item)
```
  {% else %}
```javascript
>> greetings.forEach(function(item, index, array) {
    console.log(item, index);
});
```
{% endcase %}

{% case page.lang %}
  {% when "ruby" %}
```ruby
> puts(greetings.include('सलाम'))
=> true

> puts(greetings.include('अलविदा'));
=> false
```
  {% when "python" %}
```python
>>> print(greetings.index('सलाम'))
0
>>> print(greetings.index('अलविदा'));
-1
```
  {% else %}
```javascript
>> console.log(greetings.indexOf('सलाम'));
0
>> console.log(greetings.indexOf('अलविदा'));
-1
```
{% endcase %}



* यदि हमें 1 से 100 तक की संख्याओं की सूची बनानी हो तो कैसे बनाएंगे?
* numbersUpto नाम की एक जगह बनाएं जो 1 से लेकर दी गई संख्या तक की संख्याओं की एक सूची बना कर दे। {% case page.lang %}
  {% when "python" %}
```python
>>> define numbersUpto(start, end):
...     numbers = []
...     while start <= end: 
...         ?
>>> print(numbersUpto(10))
```
  {% else %}
```javascript
>> let numbersUpto = function(start, end) {
    let numbers = [];
    while (start <= end) {
        ?
    }   
}
>> console.log(numbersUpto(10));
```
{% endcase %}
* इसको चला कर देखें क्या आता है। {% case page.lang %}
  {% when "python" %}
```python
>>> for item1 in greetings:
...     for item2 in greetings:
...         print(item1, item2)
```
  {% else %}
```javascript
>> greetings.forEach(function(item1, index1, array1) {
    greetings.forEach(function(item2, index2, array2) {
        console.log(item1, item2);
    });
});
```
{% endcase %}

* पिछले सवाल में कुछ लाईनें आती हैं जिनकी शायद हमें जरूरत ना हो, यदि हमें उनको हटाना हो तो क्या कर सकते हं। {% case page.lang %}
  {% when "python" %}
```python
>>> for item1 in greetings:
...     for item2 in greetings:
...         if ?:
...             print(item1, item2)
```
  {% else %}
```javascript
>> greetings.forEach(function(item1, index1, array1) {
    greetings.forEach(function(item2, index2, array2) {
        if (?) {
            console.log(item1, item2);
        }
    });
});
```
{% endcase %}

* 1 से 11 तक की संख्याओं को खुद से तीन बार गुणा करके एक सूची बनाएं। {% case page.lang %}
  {% when "python" %}
```python
>>> listOfNos = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
>>> listOfCubes = []
>>> for item in listOfNos:
...     listOfCubes.append(?)
```
  {% else %}
```javascript
>>  let listOfNos = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
>>  let listOfCubes = [];
>>  listOfNos.forEach(function(item, index, array) {
        listOfCubes.push(?);
    });
```
{% endcase %}

* getListOfCubes नाम की एक जगह बनाएं जो दी गई संख्या तक की सारी संख्याओं के घनों की एक सूची बना कर दे| {% case page.lang %}
  {% when "python" %}
```python
>> def getListOfCubes(n):
...    ?
>> list = getListOfCubes(11)
>> print(list[len(list) - 1]);
1729
```
  {% else %}
```javascript
>> let getListOfCubes = function(n) {
    ?
}
>> let list = getListOfCubes(11);
>> console.log(list[list.length-1]);
1729
```
{% endcase %}

यह एक function है जो हमें 9999 तक की सभी ऐसी संख्याएं बता देता है जो 2 संख्याओं के घनों से बनती हैं। 
{% case page.lang %}
{% when "ruby" %}
```ruby
> def taxiNos(list)
    nos = [];
    list.each { |item1| 
        list.each { |item2|
            sum = cube(item1) + cube(item2);
            # यदि sum चार अंकों तक का ही है और अभी तक नहीं मिला है
            if sum <= 9999 and nos.include?(sum) == false
                nos.push(sum)
            end
        }
    }
    return nos
end
> taxiNos(numbersUpto(1, 21))
```
{% when "python" %}
```python
>>> def taxiNos(list):
...     nos = [];
...     for item1 in list:
...         for item2 in list:
...             sum = cube(item1) + cube(item2)
...             // यदि sum चार अंकों तक का ही है और अभी तक नहीं मिला है
...             if sum <= 9999 && nos.indexOf(sum) == -1: 
...                 nos.append(sum)
...     return nos
>>> taxiNos(numbersUpto(1, 21))
```
  {% else %}
```javascript
>> let taxiNos = function(list) {
    let nos = [];
    list.forEach(function(item1, index1, array1) {
        list.forEach(function(item2, index2, array2) {
            let sum = cube(item1) + cube(item2);
            // यदि sum चार अंकों तक का ही है और अभी तक नहीं मिला है
            if (sum <= 9999 && nos.indexOf(sum) == -1) {
                nos.push(sum);
            }
        });
    });
    return nos;
}
>> taxiNos(numbersUpto(1, 21))
```
{% endcase %}



* Taxicab(n) नाम का एक function बनाएं जो वो सबसे छोटी संख्या बताए जो n अलग-अलग तरीकों से 2 संख्याओं के घनों को जोड़कर बनती है। {% case page.lang %}
  {% when "ruby" %}
```ruby
> def Taxicab(n)
>     ?
=> :Taxicab
> Taxicab(2)
1729
```
  {% when "python" %}
```python
>>> def Taxicab(n):
...     ?
>> Taxicab(2)
1729
```
  {% else %}
```javascript
>> let Taxicab = function(n) {
       ?
}
>> Taxicab(2)
1729
```
{% endcase %}


श्रीनिवास रामानुजन ऐसी संख्याऐं बिना कंप्यूटर जी के आसानी से ढूंढ लेते थे और उनके लिये शायद हर संख्या खास थी। आज वो हमारे बीच तो नहीं, पर हमारे साथ बात करने के लिये कंप्यूटर जी तो हैं।

और जानने के लिये हम ये वेबसाईट देख सकते हैं।
* Structure and Interpretation of Computer Programs - <https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html>
{% case page.lang %}
  {% when "ruby" %}
* Ruby Documentation - <https://www.ruby-lang.org/en/documentation/>
  {% when "python" %}
* Python Docs - <https://docs.python.org/3/>
  {% else %}
* Javascript MDN - <https://developer.mozilla.org/en-US/docs/Web/JavaScript>
{% endcase %}
* Taxicab number - <https://en.wikipedia.org/wiki/Taxicab_number>
{% case page.lang %}
  {% when "python" %}
![My helpful screenshot](/assets/python.png)
  {% when "ruby" %}
![My helpful screenshot](/assets/ruby.png)
  {% else %}
![My helpful screenshot](/assets/javascript.png)
{% endcase %}

