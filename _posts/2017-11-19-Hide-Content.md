---
category: practice
---
# How to Hide your Content
1. Use proprietory, expensive & closed formats which are tied to specific software and specific operating sytems. Your content will become classified as soon as the company that made the software/operating system decides to stop supporting old versions or is unable to support itself. 
2. Safeguard your content in XML. Anyone trying to do anything with your content will need an XML parser and clever programming skills to extract the content and put it in another format.
3. Use a database with/without SQL to store your content. You will also get atomicity, consistency, integrity, durability. Never mind you don't need all that, you are getting those free. And by the way no access without username and password. 
4. Create a PDF and delete the source file. Your document will look just like the print version and also behave like one. Be assured that anyone trying to access your content programmatically will mostly fail. Even screenreaders won't be able to read your content aloud.
