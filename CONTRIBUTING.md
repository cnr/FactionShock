Contributing
============

Thank you for your interest in contributing to Factions! We appreciate all effort
and contributions. To make things go as smoothly as possible, we have a set of
guidelines to follow:

* **Before you make a PR** Open a ticket in our [issue tracker](https://github.com/drtshock/FactionShock). This will allow us
  to discuss whether or not this change is needed and if so, how to implement it. This is key for any new feature.
* **Follow the [Oracle coding conventions](http://www.oracle.com/technetwork/java/codeconvtoc-136057.html).**
  We can't stress this enough; if your code has notable issues, it may delay
  the process significantly.
* **Target Java 7 for source and compilation.** Make sure to mark methods with
  ` @Override` that override methods of parent classes, or that implement
  methods of interfaces (Java 6+).
* **Use only spaces for indentation.** Our indents are 4-spaces long, and tabs
  are gross.
* **All messages configurable.** If you're adding messages that a player can see, make sure they are configurable
  via the lang file.
* **Wrap code to a 120 column limit.** We do this to make side by side diffs
  and other such tasks easier.
* **Write complete Javadocs.** Do so only for public methods, and make sure
  that your `@param` and `@return` fields are not just blank.
* **Don't tag classes with @author.**
* **Make sure the code is efficient and not duplicate.** [Rubber Duck Debugging](http://www.rubberduckdebugging.com).
* **Keep commit summaries under 70 characters.** For more details, place two
  new lines after the summary line and write away!
* **Test your code, please.** We're not interested in broken code, for the obvious reasons.
* **Do not touch version.** We will bump versions when ready.
* **Do not comment out blocks of code.** We have version control for this.
* **Use a new branch for the PR.** Something related to the PR. So if you were PRing a new Economy system, your branch
  could be `neweconomy`.
* **New line at the end of every file** Also a new line after class declaration before members.
* **Need help or have questions?** Join [#drtshock on Espernet](http://webchat.esper.net/?channels=drtshock) to chat with us.

Cashmoney
--------
This project is currently free and will always be open source. If/when binaries are sold, major contributors can talk to @drtshock
about potential compensation. All contributors will be allowed to run binaries without purchasing.

Checklist
---------

Ready to submit? Make sure you've done all of the following:

1. Have all tabs been replaced into four spaces? Are indentations 4-space wide?
2. Have I written proper Javadocs for my public methods? Are the @param and
   @return fields actually filled out?
3. Have I `git rebase`d my pull request to the latest commit of the target
   branch?
4. Have I combined my commits into a reasonably small number (if not one)
   commit using `git rebase`?
5. Have I made my pull request too large? Pull requests should introduce
   small sets of changes at a time. Major changes should be discussed with
   the team prior to starting work.
6. Are my commit messages descriptive?
7. Did I commit these changes to a new branch to use for the PR?
8. Does my code follow style and conventions?

You should be aware of [`git rebase`](http://learn.github.com/p/rebasing.html).
It allows you to modify existing commit messages, and combine, break apart, or
adjust past changes. If you are not, then just ask for help!

Code Style
-------

Do this:

```java
public class SomeClass {

    private Object object;

    /**
     * Does math.
     */
    public void doMath() {
        a += c + d;
        a = (a + b) / (c * d);

        while (d++ = s++) {
            n++;
        }
        printSize("size is " + foo + "\n");
    }
}
```