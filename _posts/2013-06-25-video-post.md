---
layout: post
title: "A Post with a Video"
description: "Custom written post descriptions are the way to go... if you're not lazy."
tags: [sample post, video]
comments: true
share: true
---

<embed src="http://player.youku.com/player.php/sid/XMTY1NTM5NjM2/v.swf" allowFullScreen="true" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" type="application/x-shockwave-flash"/>

Video embeds are responsive and scale with the width of the main content block with the help of [FitVids](http://fitvidsjs.com/).

Not sure if this only effects Kramdown or if it's an issue with Markdown in general. But adding YouTube video embeds causes errors when building your Jekyll site. To fix add a space between the `<iframe>` tags and remove `allowfullscreen`. Example below:

{% highlight html %}
<embed src="http://player.youku.com/player.php/sid/XMTY1NTM5NjM2/v.swf" allowFullScreen="true" quality="high" width="480" height="400" align="middle" allowScriptAccess="always" type="application/x-shockwave-flash"/>
{% endhighlight %}
