# 462-Blog

### Introduction

  Hello! My name is Ian Dudderar and I am a senior CS major at College of Charleston. I recently took 362 with Dr. Bowering last semester (Fall 2020), and that was my only experience using GitHub. I will say that while I still feel very new to the platform and its uses and operations, I feel confident I can take what I learned in the previous course and apply it to this one so that I may continue learning.


---

### Reflections on Open Source in Today's World

  Josip Almasi's article "Why I Rewrote my Open Source Virtual Reality Server" dives into one of the major issues with modern VR development companies, as well as explains his solution. In a world where everything is always about money, he believes that issue has leaked into software design and in this particular situation the development of the VR industry. Comapnies wish to lock down developers faster and longer than their competitors so that they may win the ongoing race to distribute more product and make more money. In another unforunate series of events, we live in a world where data is a heavily mainlined product among an incredible amount of different industries, and this one is no different. Some VR headsets will track a ridiculous and unnecessary amount of your biometric data and immediately sell it off to any private organization. By creating his own open source VR server, Almasi has created a safe and private enrionment for his young children and family to all interact together and enjoy the outstanding modern technology the world has to offer, without worry that their privacy is being breached. 

  Meanwhile, Emily Shannon's [article](https://opensource.com/article/17/10/enable-update) highlights the Duke University eNable group which revolves around using open sourced software to assist in the creation of 3D-printed prosthetics for amputees. The article lists multiple modular devices which have been created and loaded with different open-sourced software to assist a wide range of people all over the world, including a young child in Milot, Haiti. To me it is so neat to see the type of open sourced programs that are available out there, whether it be to help a hand pinch or an arm move. In Chris's specific case, the young boy from Haiti, they utilized a design called the Gripper Thumb Hand. The fact that these types of software exist out in the internet for anyone to use is absolutely incredible and a wholesome and wonderful use of modern technologies. Using the software, the Duke eNable team was able to produce a 3D-printed plaster prototype and eventually come up with a final device that allows Chris to use his new arm with very few limitations. They were even able to provide him with spare parts. How neat is that!
  
  
---
  
  ### This Bugs Me
  
  On the sugarlabs github, it would appear one of the oldest bug reports comes from over 3 years ago on Feb. 1st, 2018. The documenter describes a glitch in which the copy and paste function is having an issue working properly. Apparently if one starts up the desktop and copies and paste a single block of text, it works as intented. However, if one should copy one line of text, and then copy another before pasting, the final result will not paste, and actually nothing will be pasted. If I can be frank I have absolutely no idea what would cause something like this. Perhaps when the new text is copied, the old text is deleted from the clipboard, but it is never properly replaced by the new text. My theory for why it has not been resolved is that perhaps it is not a groundbreaking issue. If copying two things to the clipboard nulls them both, they could just recopy the most recent to make it work properly again. Most users probably just assume they did not select 'copy' properly, so when they do it again it works fine.
    
   Upon scouting out some of the more recent bugs, it appears there is a commonly seen error that goes into effect when users attempt to view a specific help page. There is supposed to be an activity help page that can be accessed by pressing alt+shift+H, however this takes you to a page with a bad gateway 502 error. I was in fact able to recreate this issue, as it was super simple, and it appears the devs are already aware of the problem and mentioning different possible fixes. Doing this exercise really demonstrated to me how important it is to properly document any located bugs because reading through some of the posts was very confusing as lots of them were difficult to follow and not written with the guidelines shown.
   
   Attempting to triage the bugs in this software proved to be a challenge. Many of the bugs seem trivial to me, an outsider, and therefore I do not know how to rank them, or estimate the time or effort it might take to fix one. Many of the bugs are not well documented, and instead are users simplying saying something "is broken". It's all kind of funny to read after reading the information in the TOS exercises, as it feels like I am quickly learning the importance of the reading, due to the real-world difficulties being demonstrated by poorly documented issues.
   
---

### What's Happening?

  For my article, I chose to read "Right Code" by Gerard Holmann, in the IEE Software Magazine. I am very afraid of planes and plane crashes by nature, so this article immediately grabbed my attention. Large mechanical failues due to small software errors while increasingly rare, are always tragic and spur up major conversation. It appears no matter how much the importance of proper testing and coding is pushed, human error will always find a way to show through, and I do not envision a world where this does not occur. After two of Boeing's new 737 MAX airplanes crashed, a report was published placing the blame on multiple parties and a sequence of bad practice, not just one simple fault. After a test failure of Boeing's CST Starliner system, NASA discovered the issue was due to many software bugs, calling into question the entirety of the company's testing process. The issue is that it is very difficult to come up with a single remedy that will solve any and all problems.
  
  Something interesting that stands out to me is the article's mention that oftentimes reliability is reached through redundancy. Creating multiple methods to accomplish the same task in independent manners so that should one fail, backups are available. This seems like such an obviously inefficient way of doing things,  yet at the same time makes perfect sense to me, as in some cases you would rather be safe than sorry. It goes on to mention that by increasing assertions in code may correlate strongly with fewer faults. As I have only recently learned what assertions are in regards to coding, this was intriguing to read about.
  
  As far as testing goes, the author states that tests should stemp from the requirements that prompted the codes creation, not a predetermined structure in a control-flow graph. Tests should handle a range of cases that both have expected results as well as violate certain rules. 
   
  
---

### Stupid or Solid?

  In the world of object oriented programming, the term STUPID may refer to an acronym that has been around for a while in order to describe some inherent issues behind poorly designed code. The letters stand for Singleton, Tight Coupling, Untestabilitiy, Premature Organization, Indescriptive Naming, and Duplication. As we dive deeper into these categories, we can see the negatives of each and become aware of why they should be avoided. The singleton pattern identifies a well-known pattern design in which a class is created in order to create a single object. While it can be beneficial, overuse of this can cause many problems and may lead to tight coupling. Tight coupling should be avoided so that separate program modules do not rely on each other. If you wish to make a change in a specific module, you do not want to be required to make changes in another as well. Should this occur, it will make testing very difficult, and may be an indicator of untestability. Everyone knows the importance of thoroughly testing code to be aware of any faults or potential issues. If your program is designed in a way that makes testing difficult, you're going to have a bad time. Moving forward, premature optimzation may cause someone to spend a lot of time perfecting something that does not need to or is not ready to be perfected. Code is constantly transforming and changes are always being made, therefore it may be a large waste to spend a big effort perfecting something that will only be altered in the future. This article goes on to make an important point regarding indescriptive naming. Words are for people, not for computers. It makes no sense to abbreviate variables or classes, as instead they should be given clear names and descriptors so that other people may understand them. The final letter in STUPID stands for duplication, and touches on the notion that there is no need to repeat code if it is unnecessary. Make things easier for yourself.
  
  
  On the flip side, the mnemonic SOLID may help us remember a collection of good principles and guidelines. Beginning with the Single Responsibility Principle, we learn that every class should have only one responsbility. Do not assign multiple jobs to a single class, as there is no need to overload a class with too many different responsibilities. The Open/Closed principle refers to the notion that software should be open for extension but closed for modification. In other words, variables should be made private, and getters and setters exist only where needed. The L in SOLID indicates the Liskov Substitution Principle, which says objects need to be able to be replaced by subtypes without making the program incorrect.Furthermore the interface segregation principle states that many speficic interafaces are superior to one giant one derived for many general purposes. You do not want to be obligated to impliment methods that you wont end up using. This helps to prevent coupling which we talked about earlier. Lastly, the dependency inversion principle enforces two guidelines; abstractions should not depend on details, and vice versa. 

