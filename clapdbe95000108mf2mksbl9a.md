# Got your first Dev job? Cognitive overload and how to avoid doing the same mistakes

Do you remember when you were driving a car for the first time? How new everything felt and how it seemed it was all too much to handle at once? You had to pay attention to the other vehicles, to navigate where you wanted to go, to shift gears, even to turn the steering wheel so you didn't crash...
Welcome to cognitive overload!

But really, what is it? Cognitive overload is when we're getting too much info that we need to act on. That might paralyze us or make us significantly slower while making unnecessary mistakes in the process.

# Starting a new job with little experience
I felt similarly overwhelmed when I started my first remote back-end web developer job a year ago. I had very little experience at the time, just 9 weeks of boot-camp and everything was new to me.

I had to go through the on-boarding, initialize all the projects I would be working on, learn how our git flow works, who and how to ask for help when I get stuck, read and apply all of our cookbooks... and not to forget, I had to start contributing to our projects.

I felt confused, overwhelmed and scared that I wouldn't be able to learn all the things fast enough. That I wouldn't be able to contribute.

Seems familiar to you? Do you fear the same? Continue reading. 

## How to get better faster?
Most of the things mentioned above are relatively simple procedures and principles. The problem is, there are a lot of them and they are hard to remember and apply all together in the beginning. Hence the cognitive overload.

But What if I told you that you don't have to do everything right immediately in the beginning? You're not driving a car. You  have time to think about what you're doing. You can even crash with little consequences. 

But repeated crashing (repeating the same type of mistakes all over again) isn't welcomed. 

Why not? Because someone more experienced than you has to help you and clean up your mess after you. Experienced developers are expensive. Especially in small growing companies often also overloaded with work. It's much easier to hire juniors than seniors. Don't be the junior that makes their work harder.

**But really, how exactly do I get better faster?**

## **Use the checklist [Luke](https://use-the-index-luke.com/)** 

![Screenshot 2022-10-27 at 13.03.08.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1668948460259/O3pITGUV4.png align="left")

1. **Start working on your projects and do actual coding** as fast as possible. That generates mistakes you can learn from.
2. When you make a **mistake** more than once (any mistake really e.g. naming of the feature on Gitlab, skipping someone in the code review flow, not migrating your database ...) **write it down to your checklist**.
3. **Before** you ask someone for help, create a merge request or do some kind of **action** that requires other people's attention. -> **Go through your list.**
4. Have you **done / avoided** everything on the **list?**
5. If **yes**. Create the merge request or ask your question and don't stress too much about it. If **not**, fix what you can **fix** before you do anything else.
6. **Go through the list from time to time** and think if you can add / remove / improve something.

### What exactly does this **checklist method** do for me?
1. **Helps** you with **your anxiety and cognitive overload**. You're basically **offloading your mistakes and fears** onto a piece of paper. That piece of paper can be processed systematically by you, not relying on your memory and not requiring help from others. This piece of paper **costs orders of magnitude less** than the time of your peers.
2. You **prevent** yourself from putting **more workload** on other (senior) people.
3. It helps you to **learn faster**. To learn from one's mistakes is one of the most effective ways to learn. You can also use the checklist as flashcards.
4. Since it helps you to **perform better** it also makes you **look better** in front of others.

### Is that all? That's all these lists are good for?
The best thing is, you can use this approach for almost everything. Not just for coding.
* Can't fall asleep? -> Make a list of things you need to do before going to bed to maximize the probability of having a good night's sleep. (shades, water by the bed, no blue light etc)
* Are you learning to play tennis? After the training make a list with all the mistakes your trainer pointed out to you. Then go through it and practice it later again alone. 
* Is your landlord ready to evict you? Sorry. This doesn't work in this case ... You can still follow the [Wolf of Wall street advice](https://youtu.be/PQleT6BtCbE?t=147) though ;)

### I still don't understand. Do you have an example of such a list?

#### Part of my back-end RoR checklist. What to check before pushing to Gitlab

* `pronto run -c develop`(*linter*)
* Is everything aligned the way it should be? (use `indent rainbow` Rubymine plugin).
* `rspec`(*testing library*) , for the whole project if project small enough
* Is all unused code in the app deleted (e.g. helper methods)?
* Is everything in the location it's supposed to be? (helpers vs models vs controllers vs services etc.) and/or
 *e.g. are icons in the correct place in the folder? Are locales in the correct place?
 * Is everything translated? Does the translation make sense?
* Do the method names represent their actions?
 * Is the naming in general consistent? e.g. variable names should reflect what's happening in the database,
any redundant spaces, empty lines etc?
* Have you created any complicated if statements? -> try using guard clauses instead.
* Is your text DRY? Refactor. If you don’t know how to refactor, ask someone for help.
* Have you used something like `user_id: user.id` instead of `user: user` ? Change it. Otherwise it adds unnecessary queries to the DB. 


### One more thing
There's a good chance others make the same mistakes as you.
What keeping a list helps you with is being able to see them all in one place and to think about possible bottlenecks in the flow your company is using. Then you can suggest improvements. 

For example the linter and indentation problems from the beginning of the list above can be automatically avoided with pre-commit / pre-push hooks.