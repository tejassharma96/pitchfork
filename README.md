pitchfork
=========
An unofficial python API for [pitchfork.com](http://www.pitchfork.com) reviews.

Installation
------------
Clone the repo and install ``beautifulsoup4`` and ``lxml``

Usage
-----

```python
>> import pitchfork

>> p = pitchfork.search('kanye west', 'my beautiful') # the title is autocompleted
>> p.album() # the full album title
u'My Beautiful Dark Twisted Fantasy'

>> p.label()
u'Def Jam / Roc-A-Fella'

>> p.editorial()[:100] # get the first 100 characters of the review.
u"Kanye West's 35-minute super-video,\xa0Runaway, peaks with a parade. Fireworks flash while red hoods ma"

# the link to the album cover image
>> p.cover()
'http://cdn4.pitchfork.com/albums/15935/homepage_large.831179e9.jpg'

>> p.score()
10.0
```
