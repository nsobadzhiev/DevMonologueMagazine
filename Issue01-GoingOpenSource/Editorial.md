## Editorial

### About this issue

This issue marks the very first publication for the [Dev Monologue][DevMonologue link] website, as well as for me as an author. I have no experience with publishing so be patient with me. The reason why I chose to switch to this format, instead of traditional blogging is that I believe it is more appealing and brings nostalgic for the past days of magazines and newspapers. Also, a whole issue is an opportunity to dig deeper into a subject and write several articles that complete each other, which is not something I found to be working very well with blog posts. So... without further adu... going open source!

### The open source world

There's a lot of discussion about open source software on the internet. It is gaining more and more positive publicity among programmers and IT guys alike. And of course it is an excellent way to both share knowledge and improve coding efficiency and quality and the same time. As a programmer, I'm lucky enough to appreciate open source both from a developer perspective, and as a consumer. 

Before I turned to the dark side of Mac OS, I was (and still am) a strong supporter of Linux. And as a linux user, I could experience the open source phenomenon as a consumer. I never got any benefit from being able to read my kernel's code, but I could still see the power of the community. A software made from the same people that use it. No corporate nonsense. It is amazing... (and/or I'm nerdy enough to appreciate it).

Naturally, talking about open source, kernel and community at the same time, I cannot ignore the notoriously hostile environment of contributing to the Linux kernel. To be honest I think it's a real shame what's happening there. And whereas I can totally understand a maintainer or an experienced developer's frustration with the code of lesser programmers, I cannot justify such agressive behaviour. Hopefully it gets better with time. 

Anyway, such large and infamous projects aside, there are many thousands of small chunks of code floating around in GitHub, just begging for your attention. And that's also amazing. You don't have to be a kernel developer, you don't have to work for RedHat or own a companing that managed to have a successful open source business plan. If you worked on something cool and thought someone might like it, just put it out there. It might get popular, it might just get 5-6 star on github, or not get viewed by anyone at all. Who cares? You're still part of the open source community.

An obvious question outside people ask about open source software is "**How can you make money when your product is just out there for anyone to see?**". It's surely a fair question. But you should also consider that software is an inherently a difficult intellectual property to protect. It's just a piece of information that you have to distribute to people. And no matter how good you obfuscate it, it's still possible to read to some extent. Cracks and pirated software are a hard evidence supporting that.

So, by being in the software business, you already need to be prepared to have other people "see" what you do. With open source, you just openly acknowledge that.
And quite frankly, the proverb that you should always hide in plain sight, also hold true. Just take a look at virtually any security/cryptho algorithm. They are all open source. Because the power or the community outweights the threat of exposing too much information.

In recent times, the business model for software companies has shifted away from the actual code. Especially on mobile, the software is not build to make money. It is build so that it popularizes the other services that make the money. For instance, the Wordpress mobile clients are 100% open source. And without a doubt that cannot hurt revenues, because no one pays for these apps, they are just designed for easier access to blogging for Wordpress users. And howadays, so many companies have the same situation - they don't make money from apps and they don't contain any trade secrets, so open sourcing cannot hurt them.

This brings us to another point. Who pays for open source? Obviously you cannot open source everything - there should be something else in your business plan that cannot be easily replicated seeing your code. For many core linux projects, it's actually companies like Canonical and RedHat that provide consulting services and/or need the linux system to be reliable enough for their other ventures. Also with the rise of "The cloud", it's easy to open source many your your software components but still provide them as a hosted service (like Wordpress).

All this reminds me of a very good article by Jonathan Zdziarski in his personal blog - [Free Software Always Costs Something][Zdziarski article].

### Why I chose this topic

As I'm writing this, I'm about to release the code of one of my pet projects into the wild. For a long time, it was in a private repo, but since it is never going to make money or make me famous, why not publish it. It's probably not going to be very useful to people, but maybe someday, someone is going to see it and check out the code to see how I resolved some issues, he or she is having. Maybe...who knows... anything can happen in this crazy world.

But before actually releasing the kraken, there are several things to consider. What license should I use... how do I handle dependancies, hoe can I transfer the repository from one place to another most easily... What do I write in the README...?


[DevMonologue link]: http://www.devmonogolue.com/ios
[Zdziarski article]: http://www.zdziarski.com/blog/?p=5948