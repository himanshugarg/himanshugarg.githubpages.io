---
categories: practice
---
Notes from Professor Hoare's Turing Award Lecture:-

The highest goal of programming language design is to enable good ideas to be elegantly expressed. (pp. 3)

In that design I adopted certain basic principles which I believe to be as valid today as they were then. 
1. security
2. brevity of the object code produced by the compiler and compactness of run time working data
3. the entry and exit conventions for procedures and functions should be as compact and efficient as for tightly coded machine-code subroutines.
4. The compiler should use only a single pass. (pp. 3-4)

I can still recommend single-pass top-down recursive descent both as an implementation method and as a design principle for a programming language. First, we certainly want programs to be read by people and people prefer to read things once in a single pass. Second, for the user of a time-sharing or personal computer system, the interval between typing in a program (or amendment) and starting to run that program is wholly unproductive. It can be minimized by the high speed of a single-pass compiler. Finally, to structure a compiler according to the syntax of its input language makes a great contribution to ensuring its correctness. (pp. 5)

That was my second language-design proposal. I am still most proud of it, because it raises essentially no problems either for the implementer, the programmer, or the reader of a program. (pp. 6)

I impressed upon all the programmers involved that this was no longer just a prediction; it was a promise; if they found they were not meeting their promise, it was their personal responsibility to find ways and means of making good. (pp. 8)

“You know what went wrong? You let your programmers do things which you yourself do not understand” (pp. 9)

We first listed the recent major grievances of our customers: Cancellation of products, failure to meet deadlines, excessive size of software, ‘…not justified by the usefulness of the facilities provided,’ excessively slow programs, failure to take account of customer feedback; Earlier attention paid to quite minor requests of our customers might paid us great dividends of goodwill as the success of our most ambitious plans. (pp. 9)

Our main failure was over-ambition. ‘The goals which we have attempted have obviously proved to be far beyond our grasp.’ There was also failure in prediction, in estimation of program size and speed, of effort required, in planning the co-ordination and interaction of programs, in providing an early warning that things were going wrong. There were faults in our control of program changes, documentation, liaison with other departments, with our management, and with our customers. We failed in giving clear and stable definitions of the responsibilities of individual programmers and project leaders. (pp. 10)

Told the team leader to visit the customers to find out what they wanted; to select the easiest request to fulfil, and to make plans (but not promises) to implement it. In no case would we consider a request for a feature that would take more than three months to implement and deliver. The project leader would then have to convince me that the customers’ request was reasonable, that the design of the new feature was appropriate, and that the plans and schedules for the implementation were realistic. Above all, I did not allow anything to be done which I did not myself understand. (pp. 11)

There are two ways of constructing a software design: One way is to make it so simple that there are obviously no deficiencies and the other way is to make it so complicated that there are no obvious deficiencies. (pp. 13)

If our basic tool, the language in which we design and code our programs, is also complicated, the language itself becomes part of the problem rather than part of its solution. (pp. 14)

Almost anything in software can be implemented, sold and even used given enough determination. There is nothing a mere scientist can say that will stand against the flood of a hundred million dollars. But there is one quality that cannot be purchased in this way – and that is reliability. The price of reliability is the pursuit of the utmost simplicity. (pp. 15)

If you want a language with no subsets, you must make it small. (pp 16)

An unreliable programming language generating unreliable programs constitutes a far greater risk to our environment and to our society than unsafe cars, toxic pesticides, or accidents at nuclear power stations. Be vigilant to reduce that risk, not to increase it. (pp. 17)

See [Essays in Computing Science, C.A.R. Hoare](http://delivery.acm.org/10.1145/70000/63445/cb-ecs-hoare.pdf?ip=103.27.8.45&id=63445&acc=ACTIVE%20SERVICE&key=045416EF4DDA69D9%2EF8E7F338DF557316%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35&__acm__=1517289141_7d8a8887c1da90d258956a89ba882fc6)
