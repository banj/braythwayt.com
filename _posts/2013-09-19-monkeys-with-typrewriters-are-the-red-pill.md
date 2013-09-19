---
layout: default
title: Monkeys with Typewriters are the Red Pill
tags: [noindex]
---

### preamble

For the most part, I avoid speaking at conferences. I'm shy and suffer from [Impostor Syndrome][^is]. Watching talks from accomplished people like Sandi Metz or Charles Nutter, I feel very intimidated. I have a real fear that someone will stand up and point out that I have nothing to say and I'm just babbling feel-good platitudes.

[![Nordic Ruby](http://farm4.staticflickr.com/3794/9026031742_931f2c5760_z.jpg)](http://www.flickr.com/photos/elabsse/9026031742/)

[^is]: The **impostor syndrome**, sometimes called **impostor phenomenon** or **fraud syndrome**, is a psychological phenomenon in which people are unable to internalize their accomplishments. Despite external evidence of their competence, those with the syndrome remain convinced that they are frauds and do not deserve the success they have achieved. Proof of success is dismissed as luck, timing, or as a result of deceiving others into thinking they are more intelligent and competent than they believe themselves to be.

The last two were particularly stressful. At [Nordic Ruby](http://braythwayt.com/2013/06/18/nordic-ruby.html), I talked about the possibility that Ruby is sliding into irrelevance, and although it looks healthy, it is in the same position as Microsoft a few years ago: Hamstrung by its own success. At [BaRuCo](http://www.baruco.org), I went further and questioned whether programming-as-it-is-spoke is also becoming irrelvant. Or more specifically, why the kinds of things that fascinate me are irrelevant.

I can't fault myself for sincerity: If a man suffers from imposter syndrome and he gives a talk about his own irrelevance, you can trust that the talk is from his heart!

So here are my thoughts, laid out with the metaphor I used in my slides.

[![Troop](http://farm7.staticflickr.com/6024/5888927678_9b2c9b8e14_b.jpg)](http://www.flickr.com/photos/doug88888/5888927678/)

## monkeys with typewriters

Imagine that we have  lots of monkeys, lots and lots and LOTS of monkeys. And typewriters. Lots and lots of typewriters! You know how it goes, they randomly bash on the typewriters, and given enough time, they produce the works of Phil Dick and/or Antoni Gaudi.

It's an important exercise to recognize that the number of monkeys needed to randomly recreate, say, a page of Phil Dick's short story "Second Variety" is intractably huge. But as huge as that number may be, it's *dwarfed* by the size of the real problem with putting monkeys to work generating ideas: The good stuff is buried by the crap.

Generating the works of Phil Dick isn't the problem, the problem is *recognizing* the works of Phil Dick amongst the pages of dreck, the pages describing baseball games, and the pages recounting acrimonious exchanges of tweets between trolls and their victims, and everything else that could fit on a page.

After all, for every page containing:

> Furuike ya 
> kawazu tobikomu 
> mizu no oto

There are millions, or even billions, containing stuff that is "not even wrong," such as:

{% highlight ruby %}
def andand (p = nil)
  if self
    if block_given?
      yield(self)
    elsif p
      p.to_proc.call(self)
    else
      self
    end
  else
    if block_given? or p
      self
    else
      MockReturningMe.new(self)
    end
  end 
end
{% endhighlight}

Sure, we don't really have enough monkeys, but the problem of the monkeys isn't really *interesting*. We can breed more monkeys, we can make smarter monkeys, we can make faster typewriters. Just ask Charles Nutter, if your typewriter is holding you back, he has one that isn't broken you can use for free. Inevitably, we get more and more monkey-output with every passing year whether we like it or not.

But no matter what we do, we still can't sort the good from the bad, the `andand` from the `try`. Think of it this way: This is the "spam vs. ham" problem, a/k/a [Document Classification](https://en.wikipedia.org/wiki/Document_classification).

## the ruby-red pill

You know the meme: The "red pill" is the one that tells us uncomfortable truths, but without facing the truth, we are slaves to our illusions. Only by facing the truth can we work to set ourselves free. The red pill is a real Faustian Bargain. If you take the blue pill, you are a slave, but a happy slave. Once you take the red pill, you know you are a slave, and now you must sacrifice and hurt and work to earn true freedom.

