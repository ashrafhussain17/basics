Actual Link: https://www.reddit.com/r/programming/comments/565i1n/google_interview_university_multimonth_study_plan/d8gr17k/

As an actual Google developer (mostly self-taught, no less), this list seems mostly OK, but sort of amusingly wrong in some places.
Endianness is unlikely to come up in an interview or on the job. If it does, just understanding byte-level endianness is enough. (The umd.edu page is pretty good, though.)
Binary search is great.
No one cares about 1's complement. Everything you're likely to encounter is 2's complement these days, and everyone pretty much assumes that.
In general, knowing bit tricks (counting bits, rounding to next power of 2, etc.) should be completely unnecessary. Google specifically bans questions that have a) tricky answers that b) someone can learn by rote. (And on the job, if you ever need one of those, you just use the library that someone else already wrote.) You should know basic bitwise operations, like and, or, xor, not.
Knowing a lot about trees is good. Knowing about graphs in general is good. You shouldn't need to know how to implement a red-black or AVL tree off the top of your head. I don't actually know what splay trees, 2-3 trees, or 2-3-4 trees are, so.
No one should ever ask you to implement a sort, and you should never have to implement one of your own on the job. If, for some bizarre reason, you do have to implement a sort, there are plenty of places to look it up. You should know the O() runtime of quicksort, merge sort, heap sort, and radix sort, and you should know when radix sort is actually usable.
"Recursion" should be something that is woven through most of the rest of the curriculum, but it is definitely something you should understand.
"Know about the most famous classes of NP-complete problems, such as traveling salesman and the knapsack problem, and be able to recognize them when an interviewer asks you them in disguise." -- FWIW, no interviewee ever noticed I was asking an NP-complete problem (subset sum), even when it was undisguised; not even when I called it by name. (I never cared, and never marked candidates down unless they ignored my repeated requests to just get something down, and not worry about making it fast.)
"Know what NP-complete means." In my experience, most devs don't -- it actually means something like "a problem that can be mapped from any other NP-hard problem, and which can only be solved in exponential time, but whose answer can be verified in polynomial time." In practice, most devs seem to think it means "any problem that takes exponential time to solve."
System Design, Scalability, and Data Handling shouldn't come up if you're interviewing for a junior dev position.
You shouldn't need to know any Google-specific stuff. You definitely don't need to know how Google search works, nor anything about AI/ML.
Unicode shouldn't come up in an interview, but it's very useful to understand for day-to-day work.
Maybe half of Google devs use Emacs or Vim. AFAICT, there is no real productivity difference between users of Emacs, Vim, Eclipse, or other tools, despite what Yegge says.
Unix command-line tools are nice to know, but won't land you a job, and plenty of Google devs don't know them very well.
DO NOT LEARN UML. NO ONE USES UML. NO ONE SHOULD USE UML. Seriously, I've never seen anyone outside of academia actually use UML. If you did use UML for something, your peers would have no idea how to read it.
Be very, very careful with design patterns. They are descriptive observations of code, not prescriptive patterns of code. That said, dependency injection is probably the #1 design pattern to understand, and is missing from the list.
Very few devs (even Google devs) can implement system routines. I wouldn't worry about them if your goal is just to get a job.
From the "additional learning" section:
You should absolutely understand the basics of inter-process and inter-machine messaging. You shouldn't need to know the specifics of any framework, though.
You should absolutely know about Bloom Filters before you go on your interview.
Don't bother to learn Go, unless you are placed on a Go-using team within Google.


More:

1. PoisnBGood 31 points 7 months ago 
Also a Googler and agree with all of this but wanted to clarify one thing. Not knowing how to program sorts is fine, but do know how the defining steps in merge sort, quick sort, and insertion sort as well as others work. Often times questions will be asked in such a way that you are working with sorted or nearly sorted data, and the next step is to merge or insert data. Knowing what to do here is important. Saying that you'd combine two sorted lists and then resort them isn't a good answer.

2. oridb 11 points 7 months ago 
No one should ever ask you to implement a sort
I was asked to implement a modified sort when I interviewed with Google. And I think it was a good question, even though I didn't get the optimal solution. (Yes, I did get the offer, although several years later I'm at Facebook now).
Other than that, yes, I completely agree.