---
layout: post
title: Don't Plan to be Efficient
---



## Early value vs Efficiency

Here is my explanation of why we should be thinking, when planning, of delivering value, rather than being efficient.

We sometimes hear people (developers, product people, business people) say things like: “We shouldn't implement the simplest thing that will deliver the value.  If we do that, we know that we'll throw it away, because of this future upcoming story.  It would be better to implement the feature in a more complex way; that way, when we come to do the future upcoming story, we'll have taken a more efficient path to delivering it.”  This is wrong according to XP.  It is wrong because:
    
1) It doesn't take into account the value of delivering value early
2) It doesn't take into account that evaluation of value is riskier further into the future

Let's unpack this a bit.

Suppose that we have some product features, A and B, which the business values.  We decide that
- we can deliver A by doing steps a1, a2 then a3,
- and we can deliver B by doing a1, a2, b1 then b2. (I.e. the first 2 steps are the same for A and B).

And then we notice that
- we could also deliver A by doing a1, a2 then b1
- b1 is more expensive than a3.

So, we have the choice of how to deliver A and B
- i)  a1, a2, a3 (A delivered), then b1, b2 (B delivered)

or

- ii)  a1, a2, b1 (A delivered), then b2 (B delivered)

Clearly ii) is better, because we don't do a3 and then throw it away, so we've delivered B more efficiently, right?  Wrong!

First: we're not certain that we will be asked to do B.  If it turns out that, by the time we've finished a1, a2, b1, that business priorities have changed, and B is no longer valued, then we've spent (b1 – a3) more developer time on delivering A than we needed to.  Depending on how probable it is that B will be valued, we may regard the risk of spending more developer time more or less acceptable.  If B is 90% certain to be done, then we may feel more justified in doing A the expensive way (i.e. ii), than if B is 50% certain to be done.

So, second: even if B is 100% certain to be valued, we are still wrong to do A the expensive way (ii above).  This is because A is of value to the business.  By delivering A the expensive way, we've delayed the moment at which the business realises the value.  So, all the time we spend doing b1 when we could have been doing a3, is time the business is not making money from A.


**Warning!**  The following statements are your enemies, when it comes to making the right choice.
- "Well, b1 isn't *really* that much more expensive than a3, and it will mean we're in a good position to start B"
- "We know, 100% confidence, the CEO said so, that we have to do B.  It's just wasteful to do a3 and then throw it away."
- "a3 is really ugly.  If we do it, we'll be stuck with the choices we make then.  We'll be forced to do b1 based on a3.  We won't really have the courage to throw a3 away.  We should just do b1 to make sure that a3 never sees the light of day."