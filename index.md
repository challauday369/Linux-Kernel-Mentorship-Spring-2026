                                 Udaya Kiran Challa

> *"Every expert was once a beginner."* Looking back, this quote perfectly captures my Linux Kernel Spring Unpaid 2026 Mentorship journey.

For the past few years, I've worked as an embedded software engineer, building Linux-based systems and interacting with the kernel almost every day. The Linux kernel has always been the foundation of many products I worked on, yet contributing to it felt like stepping into another world.

The kernel source tree contains millions of lines of code. Every change is publicly reviewed by experienced maintainers. Every patch becomes part of a project used by billions of devices around the world.

To be honest, contributing to the Linux kernel seemed intimidating.

That is exactly why I applied for the Linux Foundation's Linux Kernel Spring Unpaid 2026 Mentorship Program.

I hoped it would give me the opportunity to learn directly from experienced developers while making real upstream contributions. Looking back now, I can confidently say it was one of the most rewarding learning experiences of my career.

---

## The Beginning

When I received the acceptance email, I was excited—and nervous.

I knew this wasn't going to be a classroom course with predefined exercises. Instead, I would be working on the actual Linux kernel alongside maintainers and contributors from around the world.

I've chosen device tree bindings and focused on **converting legacy Device Tree binding documentation into YAML schemas**.

At first glance, it sounded like a documentation conversion.

It wasn't.

---

## Discovering What "Simple" Really Means

The first thing I learned was that YAML conversion isn't about replacing one syntax with another.

Every binding describes how hardware is represented inside the Linux kernel. Before writing a schema, I had to understand:

* the hardware itself,
* how the Linux driver used that hardware,
* Device Tree conventions,
* schema validation rules,
* and existing examples throughout the kernel.

Only then could I begin writing the YAML.

Even after writing what I believed was a correct schema, another challenge appeared.

Validation.

Commands like:

```
make dt_binding_check
make dtbs_check
```

quickly became part of my daily workflow.

Sometimes a validation error pointed exactly to the problem.

Other times...

...it didn't.

I remember spending hours tracing a schema error only to discover that the actual issue originated somewhere completely different. Those moments were frustrating, but they taught me one of the most valuable lessons in software engineering:

> **Debug patiently. Don't assume the first error message tells the whole story.**

---

## My First Patch

Submitting my first patch was surprisingly stressful.

I reread every line multiple times.

I checked formatting.

I ran validation again.

Then I finally sent it to the mailing list.

Now came the hardest part.

Waiting.

Eventually, the review comments arrived.

At first, seeing multiple comments felt discouraging. I wondered if I had misunderstood the task or overlooked something obvious.

But as I read through each suggestion carefully, I realized something important.

The reviewers weren't rejecting my work.

They were helping to improve it.

That shift in mindset completely changed how I viewed code reviews.

Instead of feeling nervous when comments arrived, I started treating them as another step toward writing better code.

---

## Learning the Upstream Way

One aspect of the Linux kernel community that impressed me was its emphasis on quality.

A reviewer might suggest:

* simplifying a schema,
* removing redundant properties,
* restructuring validation rules,
* improving examples,
* or following an existing convention already used elsewhere.

Initially, I thought these were minor details.

Over time, I understood why consistency matters in a project as large as the Linux kernel.

When thousands of developers contribute, following common conventions makes the code-base easier to maintain for everyone.

I also learned that writing code is only part of contributing.

Equally important are:

* understanding feedback,
* communicating respectfully,
* explaining design decisions,
* testing thoroughly,
* and continuously improving a patch until it is ready.

---

## Progress Through the Mentorship

By the end of the mentorship, I had submitted **Nine upstream patches** out of which **Four got merged into mainline and one patch is in linux-next (at the time of publishing this blog)**. The remaining four patches are under review process.

Seeing my **First patch merged into the Linux kernel** was an unforgettable moment.

Knowing that something I had worked on would become part of the upstream kernel was incredibly satisfying.

Each review made me a better contributor than the previous one.

---

## The Value of Good Mentors

I owe a great deal of my progress to my mentors.

Shuah Khan and Campbell never focused solely on solving problems for me.

Instead, they encouraged me to investigate, understand the root cause, and learn how the kernel community approaches development.

That style of mentorship built confidence.

Instead of depending on someone else for every answer, I gradually learned how to answer many questions myself.

Looking back, that may be the most valuable lesson they taught me.

---

## Beyond Technical Skills

The mentorship wasn't just about Device Trees or YAML schemas.

It changed how I approach engineering problems.

Today, I spend more time reading documentation before writing code.

I search existing implementations before creating new ones.

I test more thoroughly.

I appreciate constructive reviews instead of fearing them.

Most importantly, I learned that becoming an open-source contributor isn't about being an expert from day one.

It's about consistently learning and improving.

---

## Advice for Future Linux Kernel Mentorship Applicants

If you're thinking about applying for an Linux Kernel Mentorship, here are a few things I wish I had known earlier:

* Don't wait until you feel "qualified." Learning is the purpose of the program.
* Read existing code before writing new code.
* Never hesitate to ask thoughtful questions.
* Review comments are opportunities, not criticism.
* Validate and test everything before sending a patch.
* Be patient. Upstream development values correctness over speed.

Most importantly, enjoy the process.

Every patch teaches something new.

---

## Looking Ahead

Although the official mentorship has ended, my open-source journey is far from over.

I plan to continue contributing to the Linux kernel, explore new subsystems, and take on increasingly challenging work.

---

## Thank You

I would like to sincerely thank my mentors, **Shuah Khan** and **Brigham Campbell**, for their guidance, encouragement, and patience throughout this journey.

I'm also grateful to the Linux kernel maintainers and reviewers **Rob Herring**, **Krzysztof Kozlowski** and **Conor Dooley**, who took the time to review my patches and provide thoughtful feedback. Every comment contributed to my growth as a developer.

Finally, thank you to the Linux Foundation for creating a program that gives aspiring contributors the opportunity to learn by doing.

This mentorship may have started with a small YAML conversion, but it ended by changing the way I think about software engineering, collaboration, and open source.

Here's to many more patches ahead.
