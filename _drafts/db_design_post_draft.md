#

Patterns we use are ways to get faster. Usually they are the result of


Usually there are good reasons for a pattern to emerge, often they start as solving a particular problem and internalising the pattern helps us all move faster because it means we don't have to know everything about everything to be able to do anything.

They let us stand on the shoulders of giants and leverage previous work to speed us up. Which is great right up until it's not.

But it is critical that as developers we understand what those assumptions actually are, so that we can know if they are being violated or if there is a better idea.

And there's no better way to do that than to remove something and think through the consequences, which brings us to the topic of today's post.

What happens if we break referential integrity?

Foreign keys exist but they aren't actual foregin keys.

Cons

- More faff in the application when creating / deleting etc
- have to manage the referential integrity ourselves

implications with indexes?

Pros

- Moving data into different data stores is possible
- Test setup becomes easier? We don't have to insert the world in order to test on table? We can just insert the child and put random ids into the foreign key columns and not have db complain about it.
- Can still join etc.



