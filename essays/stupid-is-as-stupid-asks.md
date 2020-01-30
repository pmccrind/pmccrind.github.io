---
layout: essay
type: essay
title: Stupid is as Stupid Asks
# All dates must be YYYY-MM-DD format!
date: 2020-01-30
labels:
  - Metacognition
  - Communication
  - Time Management
---

## Think before you Ask

It is something that you do everyday. In a high stress enviroment the response needed is often immediate. In an email it can be a bit longer to allow your thoughts to fully devolp from point to point and get the meat of what it is you are really asking. The point remains you ask questions every single day. Personally I think about what I need in a satisfactory response and whom I should ask to get the answer the fastest, but I never thought about how I should be asking my question. It is beneficail for both myself and the poor person who I had the unfortunate nature of badgering with my question to think about what I want to ask. This saves us both time and frustrastion going back and forth trying to get to the bottom of it. By showing my thought process with what I have done or haven't done it shows that I have put the time in to try, really try to get to my head wrapped around this issue. Below is a question that was asked in a thoughtful way showing the thought process and what they really dying to know. The other not so much.

## The Good

[Stackoverflow: Good](https://stackoverflow.com/questions/11227809/why-is-processing-a-sorted-array-faster-than-processing-an-unsorted-array)

Two different popular programming languages. The code shortened to show all relevant code start to finish for both. Specifics of what they thought was wrong and what they tired to fix it. Relevant title and all neatly formatted and largely free of grammitcal errors, additionally a summary with what their specific questions are. Below is small porition of their post:

> ## Why is processing a sorted array faster than processing an unsorted array?

```
std::sort(data, data + arraySize);

    // Test
    clock_t start = clock();
    long long sum = 0;

    for (unsigned i = 0; i < 100000; ++i)
    {
        // Primary loop
        for (unsigned c = 0; c < arraySize; ++c)
        {
            if (data[c] >= 128)
                sum += data[c];
        }
    }
```

> My first thought was that sorting brings the data into the cache, but then I thought how silly that was because the array was just generated.
> * What is going on?
> * Why is processing a sorted array faster than processing an unsorted array?
> The code is summing up some independent terms, so the order should not matter.

By going through all the trouble to sit down and think about their question and explain what they were curious about it generated over a million views and many responses. The formatting of their question also encouraged the highest voted respondant to follow the same for their reply. They top voted response went so far as to include numerous explaniations, pictures, a link to a relevant wikipedia page, and a fix for their code. All used to explain what went wrong, and more importantly why.

## The Bad

[Stackoverflow: Not so Good](https://stackoverflow.com/questions/59977462/unity-gameobject-colour-change)

This post is from the oppisite prespective. The question is stated in the title, and while they have asked what they wanted to know they did not show the due diligence of someone asking a question on an open fourm. There is no mention of what they tired, what there thought process was or even an explainiation. It is most evident that asked a poor question by the reponses listed. The first was a litany of questions trying to get more detail, the second was a link to relevant parts of the Unity API methods. The post in its entirety is shown below:

> Unity gameobject colour change
> 
> So I've been with this for a while now, and am completly stuck. How exactly can I change of the colour of a game object when it is hit by another. What I want to do is when a target is hit, for it to change colour. Any ideas?
>
> Thanks!

