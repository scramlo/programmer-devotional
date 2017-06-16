# programmer-devotional
A 365 day, crowd-sourced devotional.
## Format and Parameters
### Language
The programmer devotional is to be written in [JSON](https://www.tutorialspoint.com/json/json_quick_guide.htm). This will enable us to export to publisher formats easily, as well as create an easily accessible API for web widgets, apps, and such.
### Required Keys
To future-proof this devotional content for future publication, there are a few required keys. Note right away that personal information is required for publishing. Below are the following necessary parameters:
* Contact Information
  * Full Name
  * Phone Number (integer, include [country code](https://faq.whatsapp.com/en/iphone/21016748) without `+`)
  * Mailing Address (string, written in a common format. Will only be used for publishing purposes and is not meant to be shared via APIs)
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
{
 {"contact": {
  {"name": "Brian Scramlin"},
  {"phone": 12015550123},
  {"address": "263 Shady Lane Drive, Wabash, Indiana 46992"}
 },
 {"meta": {
  {"title": "Frameworks"},
  {"timestamp":1497578045},
  {"scripturePassage": {
   {"book": "Matthew"},
   {"startVerse": 1},
   {"endVerse": 10},
   {"version": "ESV"}
  },
  {"scriptureHighlight": {
   {"book": "Matthew"},
   {"startVerse": 1},
   {"endVerse": 2}
  }
 }
 }
}
```
## External Resources
* [How to Write a Devotional](https://www.jerryjenkins.com/how-to-write-a-devotional/)
