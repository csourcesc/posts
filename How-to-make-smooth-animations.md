---
date: 2020-05-06 18:26:22 +0200
author: delnyn
title: How to make "smooth animations" in Scratch
image: images/Smooth-Anim.png

---
_Article written by [delnyn](https://scratch.mit.edu/users/delnyn/)._

## Introduction
In Scratch, the most common way to grow a sprite is using **change size**.
<pre class="ScratchBlocks">
change size by ()
</pre>

And the most common way to move a sprite is using **glide**.
<pre class="ScratchBlocks">
glide () secs to x:() y:()
</pre>

Using these methods for animations like clicking a button or showing a logo is not really good.  
Here, i use another method, that I call "smooth animation".  
In short, a "smooth animation" is when the sprite's movement speed varies in the animation, which is better than one of the "animating" methods showed before.
Here we'll see how to make a smooth animation for changing the size of a sprite.

## Explaining by an example : changing size
First, let's set the beginning size.  
Then, we open a loop where, at each iteration, we make our sprite grow by the size you want to get minus your current size, divided by your speed.
<pre class="ScratchBlocks">
repeat (100)
change size by (((endSize) - (size)) * (speed)) 
end
</pre>

**Important** :
* The **lower is the speed**, the more you have to **repeat the loop**.
* The **speed** should be a number between 0 and 1.

**Why do we do this ?**  
Doing the current size minus the wanted size will do the difference between these two. Knowing that difference, we multiply it by a non integer number, so we divide it, to split the difference in mutliple parts, who get smaller as the animation moves on; that's what makes the "smooth" effect.  
  
Here is an example : 
<pre class="ScratchBlocks">
set size to (50)%
repeat (100)
change size by (((200) - (size)) * (0.3)) 
end
</pre>

## Do what you want !
You can now change that code to use it for something else, like the position.
<pre class="ScratchBlocks">
go to x: (beginX) y: (beginY)
repeat (100)
change x by (((endX) - (x position)) * (speed)) 
change Y by (((endY) - (y position)) * (speed)) 
end
</pre>
Now have fun with that !  
*Thank you for reading this article :3*
