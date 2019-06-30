---
layout: post
title:  "Writing a Simple Molecular Dynamics Code in C++"
date:   2019-04-14 06:40:41 -0600
categories: physics computation chemistry
comments: true
---

The Basic Idea
==============

Writing even the most basic molecular dynamics code can
quickly grow into a massive endeavor. This is probably
because it inevitably involves the mixing of topics crossing
subject boundaries between basic code and data structures to
numerical integration of the equations of motion. So while it
could be a challenge for, I'll do my best to keep thins as
simple as possible.

Classes and Data Structures
===========================

When you're working with atoms things aren't so bad. But when
we take the jump to interacting molecules, things get really
nasty really quickly. So for now we'll start with atomic
systems only. I'll expand on the code in a follow-up article
in the future.

The items which will be necessary for use in any code that does
a simulation with atoms inside of a box will include the box properties,
atom properties (mass, charge, etc.) and their dynamical variables,
i.e. the positions and velocities.

So let's start with a `Box` class.

```cpp
#include <iostream>

/**
 * The box class
 */
class Box
{
    public:
        Box();
        Box(double);
        Box(double, double, double);
        ~Box();

        int set_x(double);
        int set_y(double);
        int set_z(double);
        int set_box(double, double, double);

    private:
        int ndim;
        double dims[3]; 
}
```

But for the purposes of this tutorial you can probably
just skip this step all together. It's just a good practice
in object-oriented programming. Now we'll build

