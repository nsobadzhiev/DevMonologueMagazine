# iOS/Mac open source world

In this article, we will delve deeper into the world of open source projects, specifically for iOS and Mac. And by that, I mean mostly iOS. On Mac, many of the really good open source applications are actually cross platform and more native to Linux than Mac OS.

Going to GitHub and starting a search for either Swift or Objective-C yields mostly frameworks and chunks of reusable code. Whereas this is really useful to other developers for learning and sharing, here we will focus on complete applications (with some exceptions). Something you can actually run and see.

Lets get started and see some prime examples of the Apple open source community:

## [Artsy][Artsy website]

Artsy is definitely an exemplary company in regards to open source. Most of what they do is out in the open. It's [always on GitHub][Artsy GitHub] and it's always free and open source. They even use the MIT license, so you are free to do whatever you like with their code. 

It probably takes a lot of courage to let go of all your intellectual property like Artsy does, but I guess it worked out in the end. Even regarding this kind of structural aspect of the company, they are really open to sharing. You can find all kinds of information [on their blog][Artsy blog] about virtually any aspect of their operation.

For example, you can find their thoughts on going open source in [this article][OSS expectations article]. They bring up a lot of good points regarding the threats and opportunities of open source software. Having a management team with a technical background definitely helps selling the idea, but the text makes a very good argument about it. 

```
Companies revolve around ideas, and understanding what your core value is important. A company who make money purely off selling their apps could be easily copied, and OSS by default won't work for them. Artsy is a platform, but OSS by default can work for us because a technical platform is just one aspect of what we offer.
-- OSS expectations, Artsy blog
```

This is a really solid point, especially regarding mobile. Users are expecting to get apps for free and paid applications are getting less and less popular. Most companies don't really expect revenue from the App Stores. Their applications are solely there to complement their business. So why hide it? It's a code base specifically tailored for a propriatary service in mind and doesn't give much (if any) advantage to your compatition. Unfortunately, looking at the majority of apps in the AppStore, most companies don't seem to share my vision.

Another great contribution from Artsy to the open source world, is the way they segment their code into libraries and more specifically how they manage those library's lifecycle. Getting a chunk of code and making it reusable by turning it into a library is a great way to encourage other developers to integrate it for their own projects. But you can also say it's more about code quality than being open and sharing knowledge. And that's surely true. By no means is open sourcing only benefiting others. By thinking about the community, you also better stucture your own code. And that by itself is quite powerful. This is actually something the Artsy team talked about in their [How we Open Source'd Eigen][How we Open Source'd Eigen post] article.

```
3 months on the way we operate has changed. We're a lot more organized, and the Eigen repo is easily the most well run project on the mobile team. It has active milestones, that represent long term goals and the current sprint. We discuss a lot of the interesting cultural choices publicly on issues and in our mobile team repo. Having this app in the open, and the experience of doing so has also improved our workflow on other apps.
-- "How we Open Source'd Eigen" post, Artsy blog
```

I guess people start working differently if they know someone could be watching. It's probably the same difference between working alone in a dark room with your monitor facing the wall and working in the middle of a huge open office with everyone looking into your screen. It's just harder to hide something embarracing so you tend to avoid it.

But going back to extracting code into frameworks, Artsy does something that would make many managers cringe. When a developer commits to creating a library out of some pile of code, they do so in their own name in GitHub. Effectively, this developer owns the code, not the company. It sounds strange at first, but first of all the code is open source either way, so everyone can use it. And secondly, their idea is that even if that developers decides to leave the team, he is still the owner of that library's code. So maybe after resign, they will continue working on the code base. And since it's 100% open source, Artsy can still use it. Awesome! You can read all about that in [Issue 22  of Objc.io][Code at scale artsy article].

So, in conclusion, there's a lot we can learn about open source from Artsy. It's an excellent example of a company that is not scared of open source, but actually leverages it to create a dynamic and vibrant development environment. I didn't write much about what their business is about, but I encourange you to [go to their website][[Artsy website]], download their apps and start using their great technology.

Companies like Artsy can show us a lot about monetarising open source software and doing business in the open. I hope it inspires people to be less scared of uploading their code for everyone to see. But that's not what open source is entirely about. It's about the little people. The developers that are driven by desire to create something for themselves but also shared it with others so that everyone can use it. The projects that are not made because of money, but because writing code can be fun. Which brings us to another amazing project:

## [MiniKeePass][MiniKeePass GitHub]

Are you using a password manager? If not, you should. A lot of people nowadays use 1Password for that, but an older, and more open source alternative, is [KeePass][KeePass website]. So, why would you use it?
* It's cross platform
* It's secure
* It's awesome

And why would you not use it?
* It's not as flashy as other solutions
* Doesn't sync your database (at least out-of-the-box)

Without going too deep into a review of the product, KeePass is a really popular, cross platform password manager solution that I personally use and love. But one question remains... does *cross platform* also include mobile? That's where MiniKeePass comes in!

MiniKeePass is a mostly independant (from KeePass itself) project that brings the popular password manager to iOS and Android. It's almost exclusively written by Jason Rush and John Flanagan. It is released under GPL (General Public License). If you wonder what that means, refer to the Open Source Licenses article of this issue. Basically it's a relatively conservative license that protects the code from being used commercially in closed source projects.

The projects is not in very active development, but it is by no means abandoned. it receives updates with fixes whenever an iOS release breaks something and also gets support for new features as the iOS operating system evolves and gives applications more freedom.

Apart from the usual benefits of an open source project, I think MiniKeePass is an excellent way to learn a little bit about security and encryption. Just clone the repository and see how a world class password manager protects your accounts.

Artsy and MiniKeePass are both great showcases, but they miss one really amazing phenomenon associated with open source software. The community! One of the most powerful aspect of open sourcing your code is to leverage the power of the community and start receiving contributions from all over the world (and become famous among nerds). However, MiniKeePass is a too small project, several developers is all it needs and Artsy is too tied to its own services to benefit the people so much that they start making many pull requests. Of course, both projects have contributors, but it's not enough for a whole community.

And now, you guessed it! We can going to look into projects with a community around them (which are also nerdy enough to get my attention).

## [Kodi][Kodi website]

Kodi, or XBMC, is one of those projects that is so big that you don't know where to start. At its core, it is a media center / home theatre software. Or at least that's how it started. Howadays, it's full of so many features, that it is difficult to explain. It's compiled for almost all the platforms you can imagine, iOS included (but for jailbroken devices mostly). As far as I remember, it also had an AppleTV version several years ago (Yes, before tvOS). Kodi supports all the codecs and protocols you can imagine. It plays radio, tv, connects to (or creates) a DLNA server and is completely extendable and skinnable.

![Kodi multi device screenshot](./Resources/KodiMultideviceScreenshot.jpg)

And it's all 100% open source. A truly amazing project. Millions of people around the world are using it and looking at their [GitHub repository][Kodi GitHub], they have (at the time of writing) 480 contributors. Of course, that's across a lot of platforms, but it makes it even more impressive. It is a whole ecosystem of enthusiasts from different backgrounds, joining forces to build something beautiful. I strongly recommend looking into Kodi's organisation. The project is really commited to establishing a strong culture between its members. It's an exemplary work of maintaining projects descriptions, product landing pages, blogs and forums. Right it the README file, people can find all the important links to get them started, they have specific resources for the ones that want to start contributing and you can find all the information you need in the forums.

It is no doubt that a community doesn't just happen, it's built and maintained. And Kodi is an ecosystem that shows how that's done.

To some, open source software has a reputation of low quality. And unfortunately, often you cannot expect the same level of polish you'd find in commercial products. But this is not the case with Kodi. It is a mature project that not only manages to bring a large number of features to its users, but also delivers them with unprecedented quality and taste. You will hardly find something that doesn't work well or is not really well thought out.

Kodi's code is released under GPLv2. It's not the most permissive license but working with some many dependencies - codecs, network protocols, plugins, it is probably hard to use a more "relaxed" license.

Overall, Kodi is a much better option for your home entertainment than most (actually all) Smart TV operating systems. If you are trying to upgrade your home theatre, get an old PC or a Raspberry Pi and setup Kodi on it. Then downloaded one of the many Kodi Remote mobile applications (I definitely recommend [the official one for iOS][Kodi remote iTunes]) and get started. 

Do you remember how I wrote that we are only going to discuss complete applications earlier in this article? Yeah... I lied a little. There is one framework in particular that is really close to my heart. A framework that saved me so much work recently and was constantly amazing me how well design it was. So naturally, I have to write something about it.

## [CorePlot][CorePlot GitHub]

CorePlot is a 2D graph and chart drawing framework built for iOS, Mac OS X and tvOS. And one of not so many, I'd say. Most alternatives I've seen are targetted towards a specific plotting task and are not very generic and reusable.

CorePlot on the other hand, supports a wide range of graph types (even pie charts) and each graph is customizable in almost every aspect. And with a current version of 2.1, it is a quite mature project.

Discussing CorePlot right after Kodi, the question of community arises naturally. The project is, I think, popular, but it definitely doesn't have a whole culture around itself. It only has 20 contributors in GitHub so far. But that doesn't mean it is not welcoming to newcomers. Looking into the project description and documentation, there is very little to complain about. All the essential information like the license, contribution guide, important links and installation tutorial are very well explained and easy to follow. The documentation is auto generated with Doxygen and it leaves a lot to be desired, but the project contains a sample application which is **really** excellent. It guides you through most of the framework's features. If you want to implement something, just find a graph within the sample application, lookup its code and copy it. That simple!

The code is released under an MIT license, unlike many of the projects we saw so far, which is very cool of the authors.

So what sets CorePlot apart from others? We already saw several extremely good projects. Artsy was able to build a successful software business "in the open". MiniKeePass was an application that extended the legacy of the core KeePass community and brought an excellent password management utility to the mainstream mobile platforms. And Kodi was an entire software suite bringing all the features you might imagine into your living room's enterntainment system, and also building a massive community of loyal users along the way. What could CorePlot possible bring to the table to compete against the others?

One of the most important aspects of code reusabilty is good architecture, intuitive interface, loose coupling and high cohesion. Obviously, if we want to use the same code in different settings, it has to be abstract and very well segmented. But that's easier said than done and all developers know that. it's more of an art than a process. Many have tried and even more have failed. 

Looking back at the specific case of CorePlot, the problem that framework is trying to resolve is inherently difficult. There are lots of components in a graph and there are more types and styles of graphs that any of us can imagine. So how do you create a library that's, at the same time easy to comprehend, fully customizable and well structured? Well, I have no idea... but it seems the CorePlot authors sort of do.

The framework itself is so big and the architecture and core principles behind it so deep that it would be impossible to explain in this article. In fact, it really deserves a whole dedicated issue (coming soon?).

What I can tell you right here is that the framework does its best to give you freedom to access and customize every element in your graph and still keep a consistent inteface in order to keep the API managable and relatively easy to understand.

Not going too deeply into that, the way they achieve that is by incorporating a "style" object into most elements that you see on screen. These styles have mostly the same interface, so you always know how to change a color or increase a font size. And if that is not enough, often you have on option to substitute a CorePlot element with your own `CALayer`, effectively injecting your own visuals into the graph. This can be a lifesaver when your design requires something quite unusual and custom made.

And while we are still on the topic of layers, CorePlot is entirely CALayer-backed, which makes the graphs highly interactive and animatable.

Overall quite an enjoyable and useful framework. Even if you don't necessarily need graphs in your app, it is still worth the time checking CorePlot out and thinking about all the design choices made there. It can serve as an inspiration and example next time you need to layout the architecture for a new app.

## Others?

There are, naturally, many other really nice open source applications for iOS and Mac OS. However, it doesn't make sense to talk about all of them here. Additional projects that I was considering writing about include [Wordpress for iOS][Wordpress GitHub], [Wikipedia for iOS][Wikipedia GitHub] and [Hammerspoon][Hammerspoon website] - a desktop automation tool for Mac OS. All of those have an interesting story to tell and are an important addition to the open source world, showing that you don't need to keep your code all to yourself and still get the job done.

In in order to cut this article short before it gets too long, we will not be covering those projects. I hope that the ones we discussed were enough to get you inspired and encourage you to develop in the open. Unless you have something really special to hide, it is probably worth thinking if you can benefit from sharing your code with the world, both for the sake of helping others, and also helping yourself. Even if you cannot build a community around your product, keeping everything for the world to see, might have a highly positive effect on your business. As they say:

```
You can write much better code with a monitor facing the entire office than if you are stuck alone in a dark basement.
```


[Artsy website]: https://www.artsy.net
[Artsy GitHub]: https://github.com/artsy
[OSS expectations article]: http://artsy.github.io/blog/2016/01/13/OSS-Expectations/
[Artsy blog]: http://artsy.github.io
[How we Open Source'd Eigen post]: http://artsy.github.io/blog/2015/04/28/how-we-open-sourced-eigen/
[Code at scale artsy article]: https://www.objc.io/issues/22-scale/artsy/
[MiniKeePass GitHub]: https://github.com/MiniKeePass/MiniKeePass
[KeePass website]: http://keepass.info
[Kodi website]: https://kodi.tv
[Kodi GitHub]: https://github.com/xbmc/xbmc
[Kodi remote iTunes]: https://itunes.apple.com/us/app/official-kodi-remote/id520480364?mt=8
[CorePlot GitHub]: https://github.com/core-plot/core-plot
[Wordpress GitHub]: https://github.com/wordpress-mobile/WordPress-iOS
[Wikipedia GitHub]: https://github.com/wikimedia/wikipedia-ios
[Hammerspoon website]: http://www.hammerspoon.org/go/