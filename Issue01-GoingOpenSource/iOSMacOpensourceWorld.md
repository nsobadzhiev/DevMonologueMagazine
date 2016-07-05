# iOS/Mac open source world

In this article, we will delve deeper into the world of open source project, specifically for iOS and Mac. And by that, I mean mostly iOS. On Mac, many of the really good open source applications are actually cross platform and more native to Linux than Mac OS.

Going to GitHub and starting a search for either Swift or Objective-C yields mostly frameworks and chunks of reusable code. Whereas this is really useful to other developers for learning and sharing, here we will focus on complete applications (with some exceptions). Something you can actually run and see.

Lets get started and see some prime examples of the Apple open source community:

## [Artsy][Artsy website]

Artsy is definitely an examplary company in regards to open sources. Everything they do is out in the open. It's [always on GitHub][Artsy GitHub] and it's always free and open source. They even use the MIT license, so you are free to do whatever you like with their code. 

It probably takes a lot of courage to let go of all your intellectual property like Artsy does, but I guess it worked out in the end. Even regarding this kind of structural aspect of the company, they are really open to sharing. You can find all kinds of information [on their blog][Artsy blog] about virtually any aspect of their operation.

For example, you can find their thoughts about going open source in [this article][OSS expectations article]. They bring up a lot of good points regarding the threats and opportunities of open source software. Having a management team with a technical background definitely helps selling the idea, but the text makes a very good argument about it. 

```
Companies revolve around ideas, and understanding what your core value is important. A company who make money purely off selling their apps could be easily copied, and OSS by default won't work for them. Artsy is a platform, but OSS by default can work for us because a technical platform is just one aspect of what we offer.
```

This is a really solid point, especially regarding mobile. Users are expecting to get apps for free and paid applications are getting less and less popular. Most companies don't really expect revenue from the App Stores. Their applications are solely there to complement their business. So why hide it? It's a code base specifically tailored for a propriatary service in mind and doesn't give much (if any) advantage to your compatition. Unfortunately, looking at the majority of apps in the AppStore, most companies don't seem to share my vision.

Another great contribution from Artsy to the open source world, is the way the segment their code into libraries and more specifically how they manage those library's lifecycle. Getting a chunk of code and making it reusable by turning it into a library is a great way to encourage other developers to integrate it for their own projects. But you can also say it's more about code quality than being open and sharing knowledge. And that's surely true. By no means is open sourcing only benefiting others. By thinking about the community, you also better stucture your own code. And that by itself is quite powerful. This is actually something the Artsy team talked about in their [How we Open Source'd Eigen][How we Open Source'd Eigen post] article.

```
3 months on the way we operate has changed. We're a lot more organized, and the Eigen repo is easily the most well run project on the mobile team. It has active milestones, that represent long term goals and the current sprint. We discuss a lot of the interesting cultural choices publicly on issues and in our mobile team repo. Having this app in the open, and the experience of doing so has also improved our workflow on other apps.
```

I guess people start working differently if they know someone could be watching. It's probably the same difference between working alone in a dark room with your monitor facing the wall and working in the middle of a huge open office with everyone looking into your screen. It's just harder to hide something embarracing so you tend to avoid it.

But going back to extracting code into frameworks, Artsy does something that would make many managers cringe. When a developer commits to creating a library out of some pile of code, they do so in their own name in GitHub. Effectively, this developer owns the code, not the company. It sounds strange at first, but first of all the code is open source either way, so everyone can use it. And secondly, their idea is that even if that developers decides to leave the team, he is still the owner of that library's code. So maybe after resign, they will continue working on the code base. And since it's 100% open source, Artsy can still use it. Awesome! You can read all about that in [Issue 22  of Objc.io][Code at scale artsy article].

So, in conclusion, there's a lot we can learn about open source from Artsy. It's an excellent example of a company that is not scared of open source, but actually levarages it to create a dynamic and vibrant development environment. I didn't write much about what their business is about, but I encourange you to [go to their website][[Artsy website]], download their apps and start using their great technology.

Companies like Artsy can show us a lot about monetarising open source software and doing business in the open. I hope it inspires people to be less scared of uploading your code for everyone to see. But that's not what open source is entirely about. It's about the little people. The developers that are driven by desire to create something for themselves but also shared it with others so that everyone can use it. The projects that are not made because of money, but because write code can be fun. Which brings us to another amazing project:

## [MiniKeePass][MiniKeePass GitHub]

Are you using a password manager? If not, you should. A lot of people nowadays use 1Password for that, but an older, and more open source alternative, is [KeePass][KeePass website]. So, why would you use it?
* It's cross platform
* It's secure
* It's awesome

And why would you not use it?
* It's not as flashy as other solutions
* Doesn't sync your database (at least out-of-the-box)

Without going too deep into a review of the product, KeePass is a really popular, cross platform password manager solution that I personally use and love. But one question remains... does *cross platform* also include mobile? That's where MiniKeePass comes in!

MiniKeePass is a mostly?? independant (from KeePass itself) project that brings the popular password manager to iOS and Android. It's almost exclusively written by Jason Rush and John Flanagan. It is release under GPL (General Public License). If you wonder what that means, refer to the Open Source Licenses article of this issue. Basically it's a relatively conservative license that protects the code from being used commercially in closed source projects.

The projects is not in very active development, but it is by no means abandoned. it receives updates with fixes whenever an iOS release breaks something and also gets support for new features as the iOS operating system evolves and gives applications more freedom.

Apart from the usual benefits of an open source project, I think MiniKeePass is an excellent way to learn a little bit about security and encryption. Just clone the repository and see how a world class password manager protects your accounts.

...

Artsy and MiniKeePass are both great showcases, but they miss one really amazing phenomenon associated with open source software. The community! One of the most powerful aspect of open sourcing your code is to levarage the power of the community and start receiving contributions from all over the world (and become famous among nerds). However, MiniKeePass is too small of a projects, several developers is all it needs and Artsy is too tied to its own services to benefit the people so much that they start making many pull requests. Of course, both projects have contributors, but it's not enough for a whole community.

And now, you guessed it! We ca ngoing to look into projects with a community around them (which are also nerdy enough to get my attention).

## Kodi


[Artsy website]: https://www.artsy.net
[Artsy GitHub]: https://github.com/artsy
[OSS expectations article]: http://artsy.github.io/blog/2016/01/13/OSS-Expectations/
[Artsy blog]: http://artsy.github.io
[How we Open Source'd Eigen post]: http://artsy.github.io/blog/2015/04/28/how-we-open-sourced-eigen/
[Code at scale artsy article]: https://www.objc.io/issues/22-scale/artsy/
[MiniKeePass GitHub]: https://github.com/MiniKeePass/MiniKeePass
[KeePass website]: http://keepass.info