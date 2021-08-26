# Corinna

## RFC

This is to track the RFC for the Corinna MVP OOP proposal.

[% FOREACH template IN templates -%]
[% template.index %]. [[% template.name %]]([% template.file %])
[% END %]

**Important**: All of the above represent works in progress. Please do not
consider this the final RFC. We're writing down the shell of the RFC and will
fine-tune. Anything in the Wiki should be considered "rough drafts."

See also, [quotes from various people involved](rfc/quotes.md).

## Not a Tutorial

This is not a tutorial on OO programming. That could easily fill a book. It's
assumed you're already very familiar with Perl's built-in OO. It's very useful
if you're also familiar with Moo/se.

## Principle of Parsimony

Many things in the proposal are _deliberately_ restrictive, such as Corinna
only allowing single inheritance. This is to allow Corinna to be cautious in
not promising too much. If we later find this too restrictive, we can allow
multiple inheritance. However, if we start with multiple inheritance and
discover we don't need or want multiple inheritance, we would break existing
code by taking it away.

Any proposals to change the RFC must consider the principle of parsimony.

## This Repository

This repository is not for code. Instead, it’s to have a central place to
discuss the Corinna proposal to bring modern OO to the core of the Perl
language. 

You may be looking for the [Wiki](https://github.com/Ovid/Cor/wiki) as that
has much historical discussion of this project. However, the documents in the
`rfc/` folder will be considered the canonical ones.

[You can file issues](https://github.com/Ovid/Cor/issues) to address your
particular concerns and get feedback.

## Changes

[See the Changes file](rfc/major-changes.md).

## MVP

This work is to drive us to v0.1.0—not v1.0.0—the “minimum viable product.” The
intent is to get the subset of features we really need into the language, make
sure it’s stable, and then iterate on top of that. I don’t want us building on
top of this foundation only to discover the foundation is not stable.

I’ve been getting some pushback from people being quite insistent that if I
don‘t support one or more of the features that _they_ like to use, that it will
be so terribly hobbled that it will be of limited use to them.

Please keep in mind that if this MVP does get into core, I will have lost
control over it (yay!) and I’ll have no particularly greater voice than others.
That means:

**If this gets into the core and you want a feature, lobby for it.**

I’m not a gatekeeper. I don’t want to be a gatekeeper. I want to get modern OO
into the Perl core and the more things added to the MVP to scratch people’s
personal itches, the more bugs there will be and the less likely it is to be
stable. Let’s focus on the MVP and getting this in core.

After that, it will be up to the community to decide where it wants to go. I
will have _zero_ authority to stop things I disagree with if P5P decides to
implement them. This will effectively be a democracy. A level playing field.
If you won’t support Corinna because your personal favorite feature isn’t in
the MVP, I don’t know what to say to that. You, like everyone else, will be
able to lobby for that feature.