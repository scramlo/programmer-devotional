# programmer-devotional
A 365 day, crowd-sourced devotional.
## Format and Parameters
### Language
The programmer devotional is to be written in [JSON](https://www.tutorialspoint.com/json/json_quick_guide.htm). This will enable us to export to publisher formats easily, as well as create an easily accessible API for web widgets, apps, and such.
### Required Keys
To future-proof this devotional content for future publication, there are a few required keys. Note that personal information is required for publishing, such as a mailing address. However, so we don't post your personal information all over the web--an email address is all we will require and will contact you for a mailing address upon any publisher requests for that information. Below are the following necessary parameters:
* Contact Information
  * Full Name
  * Phone Number (integer, include [country code](https://faq.whatsapp.com/en/iphone/21016748) without `+`)
  * Email
* Devotional Meta Data
  * Title
  * Date (integer, current [unix timestamp](http://www.unixtimestamp.com/)
  * Suggested Scripture
  * Highlighted Verse
* Devotional Text
  * Devotional Body
  * Single Takeaway
  * Prayer
### Devotional Body
Consistency among the devotionals can be achieved by implementing a common format. Please, to the best of your ability write your devotional body according to the following pattern.:

> 1. Hook: An excellent lead and a compelling anecdote will grab and hold (hook) the reader’s attention.
> 2. Book: Point them to the wisdom of the Bible (book).
> 3. Look: Offer some unique way of seeing (look) how the Bible relates to his or her needs.
> 4. Took: Finally, provide takeaway (took) value.

These four sections should not be denoted or parsed, they are a general guideline to create consistency. 
### Example
```
contact
  name=Brian Scramlin
  phone n=12015550123
  email=brian@nerdspecs.com
meta
  title="Convention over Configuration"
  timestamp n=1497611964
  scripturePassage
    book=John
    version=ESV
    chapter n=6
    startVerse n=60
    endVerse n=66
  scriptureHighlight
    startVerse n=68
    endVerse n=68
devotion
  body=<p>In web development there is a principle called "convention over configuration" It means if you code according to the pattern (or convention) suggested by the framework&nbsp;you are using, everything will automagically&nbsp;work. This is different than configuring every piece of code to work with other pieces.</p><p>When Jesus taught, His words left little room for hanging on to other frameworks. What He said was difficult to accept for some, but for those who did receive His words everything all made sense in the end. Peter had the right idea declaring "Lord, to whom would we go? You have the words that give eternal life" Even if he didn't understand the "why" or "how" behind Jesus' teachings, he trusted the "who"</p><p>As an Evangelical Christian, I have accepted a&nbsp;framework. This is different than some people attempt their philosophy of life. For these people, everything one believes should be tested and approved by their personal canon (configuration). But, not me. Even if I don't know how it works that when I forgive, bless, and pray for my enemies, life is better--it automagically works.</p>
  thesis=Even if you don't understand the "why" or "how", when you take Jesus at His word your life will automagically be blessed.
  prayer=Lord Jesus, I may not always understand "why" You have called us to some things in life or "how" they will result in Your glory and our good, but I trust that when I follow everything you teach it will all work out.
```
## External Resources
* [How to Write a Devotional](https://www.jerryjenkins.com/how-to-write-a-devotional/)
