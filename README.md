[Domain Names](https://github.com/paulshorey/domain-names)

# Instructions  

In this `domain-names` folder, **`all-sorted.js`** is a list of domain name extensions. For each domain name extension, is a list of related words.  

#### I need help adding related words to each domain name extension.  

Don't worry about breaking the format too much. I am good at fixing code syntax errors. :) But do try to keep the quotes and commas and colon characters in place as they are now.  

The list of words, following the domain name extension and colon ":", are like SEO words. They are words which a site visitor may type in to search. The site visitor will be given the domain name extension as a suggestion.  
I am making an AI application, which will suggest domain names to people who search for "campus gossip .com" but it is unavailable.  
Instead, they will get suggestions like "campus.news", "campus.media", "gossip.edu", "chatter.edu".  

I will get synonyms for "college", and match them with synonyms for "edu". If they intersect, then the user's query "college..." will be paired with the domain extension "edu".  
Likewise, I get synonyms for "gossip" and match with synonyms for all domain extension. I will find that "news" shares some synonyms with "gossip". So, I will use "news". Same for "media".  

"edu": `school, education, learn, classes, study, `,  

The words do not need to be very close, because I will get synonyms of these synonyms. So, if you type in "school", you do not have to also type in "college, university, elementary school, high school". It will all match anyway.  
  
Review: If user searches for "school" or any synonym like "college, university", they will get domain extension "edu" as a response.  
  
---
  
#### So, this is an easy job. It is just time consuming.  
  
I need synonyms for about 500 of these extensions "com, net, org, gov, co, info, biz", and new ones like "lawyer, hotel, vip, win, top...".  
The longer extensions like "accountant" and "vacations" don't need many synonyms. 3 will suffice.
But the shorter ones which are not obvious, or are not a real word "top, xxx, llc, am, fm, post", need many synonyms, 10+.

Looking to fill this with about 5,000 words (500 extensions x 10 synonyms) average. 

There are actually about 800 extensions, but they don't all need synonyms. Some are Chinese, some are Russian. Some are self-explanatory like "accountant".

Please add synonyms to each extension, in any random order. I will compare the difference. I can see what changed. 

Review: each synonym is a word that the user may search (like SEO keywords). The domain extension "edu" is what the user will receive as a result. The user will receive one or many domain extensions, which match at least one of the keywords they search.

---

#### For example:

"ltd": `inc, biz, business, corporation, registered, `,
When the user types any word which is a synonym of inc, biz, business, corporation, or registered, they will get the extension "ltd".


#### Another example, "ink":

When user types in any synonym of `writing, literature, magazine, newspaper, news, media, multimedia, publish, book, author`, they will receive the domain extension ".ink".

So, to accomplish this, my list must contain the line:
"ink": `lit, writing, literature, magazine, newspaper, news, media, multimedia, publish, `,

---

## This is the file to edit:
[domains: all-sorted.js](https://raw.githubusercontent.com/paulshorey/domain-names/master/all-sorted.js)
