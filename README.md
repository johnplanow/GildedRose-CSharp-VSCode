# Gilded Rose Refactoring Kata

Hi and welcome to team Gilded Rose. As you know, we are a small inn with a 
prime location in a prominent city ran by a friendly innkeeper named 
Allison. We also buy and sell only the finest goods. Unfortunately, our 
goods are constantly degrading in quality as they approach their sell by 
date. We have a system in place that updates our inventory for us. It was 
developed by a no-nonsense type named Leeroy, who has moved on to new 
adventures. Your task is to add the new feature to our system so that we 
can begin selling a new category of items. First an introduction to our 
system:

- All items have a SellIn value which denotes the number of days we have 
to sell the item
- All items have a Quality value which denotes how valuable the item is
- At the end of each day our system lowers both values for every item

Pretty simple, right? Well this is where it gets interesting:

- Once the sell by date has passed, Quality degrades twice as fast
- The Quality of an item is never negative
- "Aged Brie" actually increases in Quality the older it gets
- The Quality of an item is never more than 50
- "Sulfuras", being a legendary item, never has to be sold or decreases 
in Quality
- "Backstage passes", like aged brie, increases in Quality as it's SellIn 
value approaches; Quality increases by 2 when there are 10 days or less 
and by 3 when there are 5 days or less but Quality drops to 0 after the 
concert

We have recently signed a supplier of conjured items. This requires an 
update to our system:

- "Conjured" items degrade in Quality twice as fast as normal items

Feel free to make any changes to the UpdateQuality method and add any 
new code as long as everything still works correctly. However, do not 
alter the Item class or Items property as those belong to the goblin 
in the corner who will insta-rage and one-shot you as he doesn't 
believe in shared code ownership (you can make the UpdateQuality 
method and Items property static if you like, we'll cover for you).

Just for clarification, an item can never have its Quality increase 
above 50, however "Sulfuras" is a legendary item and as such its 
Quality is 80 and it never alters.

## Getting Started

This kata was setup by [John Planow](https://www.linkedin.com/in/johnplanow) 
to run with [.NET Core SDK 2.1](https://www.microsoft.com/net/download/) 
using [Visual Studio Code](https://code.visualstudio.com/download). I've
deliberately included the bare minimum so your version of the toolset can
take care of the rest with a couple easy button pushes.

If you know anything about these tools, you're ahead of where I was 
when I set out to do this. If you notice anything that could be done better,
drop me a line. I'd love to hear about it. 

On the other hand, if you're brand new with these tools or to C#, fear 
not. That's half the fun! Here are a few steps to get you started:

 1. Install .NET Core SDK and Visual Studio Code (VS Code) through the
    links above
 2. Start VS Code
 3. Hit Cmd-Shift-P (Win: Ctrl-Shift-P) to bring up the command pallette
 4. Type "Install Extensions" and use the Extensions pane to install:  
   a. C# for Visual Studio Code  
   b. .NET Core Test Explorer  
 5. File &rarr; Open (or Cmd-O / Ctrl-O) and select the root folder of this
    project
 6. Expect one or more popup alerts about missing dependencies and whatnot. 
    Click the appropriate button(s) to add and/or restore them.

At this point, you should have a .NET Test Explorer pane in the left
sidebar with a test you can run, and debug icon also somewhere on the
left. Have fun!

## Who, What, Why?
Who: [@TerryHughes](https://twitter.com/TerryHughes), [@NotMyself](https://twitter.com/NotMyself)

What & Why: [Refactor This: The Gilded Rose Kata](http://iamnotmyself.com/2011/02/13/refactor-this-the-gilded-rose-kata/)

## License

MIT

## Suggested attribution

This work is by [@TerryHughes](https://twitter.com/TerryHughes), [@NotMyself](https://twitter.com/NotMyself)

The repository can be found at [https://github.com/johnplanow/GildedRose-CSharp-VSCode](https://github.com/johnplanow/GildedRose-CSharp-VSCodee)

The original repository can be found at [https://github.com/NotMyself/GildedRose](https://github.com/NotMyself/GildedRose)

Other variations can be found at [https://github.com/emilybache/GildedRose-Refactoring-Kata](hhttps://github.com/emilybache/GildedRose-Refactoring-Kata)
