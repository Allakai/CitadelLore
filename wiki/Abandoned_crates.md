---
title: Abandoned crates
permalink: wiki/Abandoned_crates/
layout: wiki
---

While out digging on the asteroid, miners and xenoarchaeologists may
occasionally stumble upon crates buried in the rock. These crates are
typically sealed with an old, reliable anti-tamper mechanism and a
deca-code lock, a mechanical lock requiring that a 4-digit code be
entered to unlock the crate. Deca-code locks have fallen out of favour
on more modern installations due to mechanical limitations on the code
that restrict the possible combinations to numbers where all four digits
are unique, and vulnerabilities where a multitool can be used to
determine how close the previously-entered code was to the correct
answer, allowing a moderately-skilled codebreaker to bypass the lock.

Cracking the code
-----------------

The deca-code lock is essentially a mastermind puzzle with 10 different
colours of pegs. In fact, it's *easier* than that, because of the
limitation that the same peg can't be used more than once in the code.

If you don't have a multitool, go and fetch one before you start.
Randomly guessing numbers has such low odds of hitting the right code
that you might as well just leave it.

Firstly, enter any four digits you like, as long as they're all
different. "1234"is a good start. Then, use the multitool on the crate -
it will give you a short explanation of how many digits in your guess
are found in the correct code (and of those, how many were in the
correct position).

Try another guess, say "5678" and take more notes. You get 10 guesses,
so your first couple of guesses should simply be to eliminate the
possible combinations that it *can't* be. For instance, if you find all
four digits in 1234 and 5678, then you know the final code does *not*
contain 9 or 0.

After that, try shifting the numbers along - 3456, for instance. If you
get a number showing in the correct position, then that must be one of
the numbers that was in an *incorrect* position in your earlier guesses,
but your priority should be finding all four of the correct numbers
first and *then* worrying about the order.

Once you get some clues that certain numbers are definitely present,
change the remaining digits about. Usually you'll end up with groups or
pairs where you know that *one* of the numbers is present. Try swapping
one of the numbers for one from the other group - if it makes no
difference, then you know they're *both* right or *both* wrong.

With a little practice, this process becomes relatively simple - you'll
probably be able to crack them in less time than it takes to persuade
security to let you "borrow" a gun.

Examples
--------

It's easier to show than to tell, so your friendly admonster fired up
his test server. We'll run through some step-by-step, with an
explanation at each stage.

### Example 1

-   1234 - 0 correct digits at correct positions and 0 correct digits at
    incorrect positions. *This is a stroke of luck. 4 digits eliminated
    immediately.*
-   5678 - 1 correct digits at correct positions and 2 correct digits at
    incorrect positions. *Now we're getting somewhere. We also know that
    the missing digit must be 9 or 0.*
-   7890 - 2 correct digits at correct positions and 1 correct digits at
    incorrect positions. *3 digits in this group too. That means the
    incorrect digit from 5678 must be 5 or 6, as we know the incorrect
    one in this group is 9 or 0. 7 and 8 are definitely present.*
-   7895 - 1 correct digits at correct positions and 1 correct digits at
    incorrect positions. ''We put in the digits we know for sure are
    present, 7 & 8, and swap out one of the ones we're unsure on for
    another one we're unsure on. We only changed the last digit, 0, for
    a 5, and it tells us there's one less correct answer. Now only does
    this tell us that 5 and 9 are *'not* in the code, as the change was
    to the correct digits it tells us that 0 is the last digit in the
    correct answer.''
-   7860 - 2 correct digits at correct positions and 2 correct digits at
    incorrect positions. *We already know 7 or 8 are in the right place,
    so 6 isn't. Let's swap them around.*
-   6870 - The crate unlocks!

### Example 2

-   1234 - 0 correct digits at correct positions and 1 correct digits at
    incorrect positions. *Decent enough start.*
-   5678 - 0 correct digits at correct positions and 1 correct digits at
    incorrect positions. *Interesting. So 9 and 0 are both present.
    Let's see if we can narrow down the other two.*
-   3456 - 1 correct digits at correct positions and 0 correct digits at
    incorrect positions. ''Doesn't tell us much yet, other than the
    position of whichever one is in this range. Let's start putting 9 &
    0 in.
-   7890 - 0 correct digits at correct positions and 3 correct digits at
    incorrect positions. ''Bingo. As the last two guesses had all four
    numbers, it can't have 1 or 2. That means 3 or 4 are correct (from
    the first guess), and knowing that means we can eliminate 5 & 6 from
    the third guess. So the code has 3 or 4, 7 or 8, 9, and 0.
-   3890 - 1 correct digits at correct positions and 2 correct digits at
    incorrect positions. ''Swapping the 7 for a 3 puts a correct one in
    the correct position - we didn't change any positions around, so
    this means the first digit must be 3. It also tells us that the 8 is
    incorrect. So the final code is 3, 7, 9 and 0 in a different order.
-   3907 - The crate unlocks!

### Example 3

Ran through this as a speedrun, probably not the optimal route. All the
italic notes were added after I'd found the answer.

-   1234 - 1 correct digits at correct positions and 1 correct digits at
    incorrect positions.
-   5678 - 0 correct digits at correct positions and 0 correct digits at
    incorrect positions. *That's handy. Last missing digits are 9
    and 0.*
-   1290 - 1 correct digits at correct positions and 2 correct digits at
    incorrect positions. *So it's 1 or 2, 3 or 4, 9 and 0.*
-   1390 - 1 correct digits at correct positions and 3 correct digits at
    incorrect positions. *All four digits confirmed, let's try the
    order.*
-   1903 - 0 correct digits at correct positions and 4 correct digits at
    incorrect positions. *So the first digit isn't 1. Next.*
-   9301 - 1 correct digits at correct positions and 3 correct digits at
    incorrect positions. ''Let's see if it's the 3. In retrospect, this
    was a bad move as 1290 had a correctly positioned digit, so I should
    have already known that 3 wasn't the 2nd digit. At least this tells
    us that SOMETHING in this guess is correct.
-   0319 - 0 correct digits at correct positions and 4 correct digits at
    incorrect positions. ''Again, confirmed that 3 isn't in the right
    place.
-   3091 - 0 correct digits at correct positions and 4 correct digits at
    incorrect positions. ''The 9 isn't the one that's right, so the last
    digit must be 0. Let's put the other digits in place - we know what
    numbers are **not** in each position from our earlier guesses.
-   9130 - The crate unlocks!

### Example 4

Another speedrun.

-   1234 - 0 correct digits at correct positions and 1 correct digits at
    incorrect positions.
-   5678 - 1 correct digits at correct positions and 2 correct digits at
    incorrect positions. *We can eliminate 9 and 0.*
-   3456 - 2 correct digits at correct positions and 1 correct digits at
    incorrect positions. *5 & 6 are probably correct. Let's confirm
    that.*
-   1256 - 1 correct digits at correct positions and 1 correct digits at
    incorrect positions. *Confirmed. Also eliminated 1 & 2, and we know
    3 OR 4, and 7 OR 8 are there.*
-   3756 - 1 correct digits at correct positions and 1 correct digits at
    incorrect positions. *This eliminates 3 & 7, as swapping them in for
    two known wrong answers produces the same result.*
-   8456 - 2 correct digits at correct positions and 2 correct digits at
    incorrect positions. *All four digits confirmed, let's try the
    order - we'll keep 4 in the same place and see what happens.*
-   5468 - 2 correct digits at correct positions and 2 correct digits at
    incorrect positions. *Something moved into the right place, and
    something that was in the wrong place moved into the right place.*
-   5486 - 1 correct digits at correct positions and 3 correct digits at
    incorrect positions. *Swapping the last two digits for a little more
    info, then plug them in where they fit the pattern...*
-   6458 - The crate unlocks!

### Example 5

Possibly lucky? Got this in less than three minutes from start to
finish. Partly through lucky guesswork, but it wouldn't have taken much
longer from that point.

-   1234 - 0 correct digits at correct positions and 2 correct digits at
    incorrect positions.
-   5678 - 1 correct digits at correct positions and 1 correct digits at
    incorrect positions. *No 9 or 0.*
-   3456 - 0 correct digits at correct positions and 2 correct digits at
    incorrect positions.
-   1256 - 0 correct digits at correct positions and 0 correct digits at
    incorrect positions. *Code is 3, 4, 7 & 8. 7 or 8 were in the right
    place. Keep one there, move the other.*
-   4873 - The crate unlocks! *Lucky guess? Maybe, but we still had 5
    more guesses to try other combinations.*
