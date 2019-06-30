--
categories: practice
--

## ABSTRACT

The current status of Indian languages on the web may best be described as “Diversity in Unity”! All Indian language scripts (except for Urdu & Sindhi) are derived from the same Brahmi Script and also share a common alphabet to a large extent. But languages like Hindustani, Sindhi use different scripts making the texts available in one script inaccessible to persons not knowing that script. Because of different scripts for different Indian languages, which otherwise share common culture, two languages can’t share language independent information with each other. When it comes to electronic media, the situation is still worse. Even the texts in the same language are font dependent making them unsharable. Though standards exist they are not followed!

In this thesis we propose solutions
* to overcome the font barrier within a language for all brahmi based
scripts.
* to overcome the script barriers across the language among all brahmi
based scripts
* to overcome the script barrier in case of Hindustani-Hindi-Urdu

The problem of font barriers within a language is because of different coding schemes followed by different font designers. While a standard coding scheme (Unicode/ISCII) exists, it is not used. Converters that can convert from the unknown encoding to ISCII can largely solve the problem. However manually coding converters is difficult and time consuming. This thesis attempts to tackle the problem of generating such converters, using two different approaches. The first approach uses a mnemonic based description of glyphs in the font. This description is used to convert a font encoded text. Accuracies of above 75% for two Telugu fonts and above 90% for three Devanaagari fonts have been obtained.  The second approach uses example based machine learning techniques to generate Finite State Transducers. These Finite State Transducers can be automatically learnt from syllable mappings of font encoded text to Unicode text. Accuracy of above 90% has been obtained when 1000 syllable mappings from font encoding to Unicode were provided.

The second problem of overcoming the script barriers across the languages may simply be solved by following the ISCII standard.  The transliteration from Urdu to Hindi makes a text written in the Perso – Arabic script accessible to those who know the Devanaagari script. Such a transliteration is non trivial because there is not a one to one mapping between Urdu and Hindi alphabets. Omission of vowel signs in Urdu which must be present in Hindi complicates the issue further. We discuss these and other issues involved in overcoming the script barriers in case of Urdu - Hindi and propose a solution to
overcome this barrier.

[PDF]({{ site.baseurl }}/pdf/thesis.3.3.pdf)
