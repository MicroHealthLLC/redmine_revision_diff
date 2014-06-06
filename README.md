## redmine_all_diff

This is a simple redmine plugin to show the diff of a revision on the revision page (redmine only show a list of modified files).

## Why?

Well, I used trac (and I still use) a lot, and I'm totally used to see the diff of a commit right there in the changeset page. Redmine would only show a list of the modified files though, and the diff itself lies deeper in the page, one more click away. 

So I searched to see if this was a feature that I didn't know how to turn on, or if not, if it was planned, or if not, if there was a plugin that could do that. Well, there's probably a plugin somewhere, but I couldn't find it.

It should be a very simple thing to implement because I could do it adding just a few lines to redmine's source code, but I had never tried to make a redmine plugin so it ended up being just a little more complicated because I had to think and search about the best way to add the stuff I needed without messing directly with any of the core classes, or else I'd end up with a plugin that only worked with a specific version of Redmine.

## Installation

From redmine directory
```bash
cd plugins
```
```bash
git clone https://github.com/mateusmedeiros/redmine_all_diff.git
```

And that's it.

I made this with redmine 2.5.1 and intended to use in 2.4.3. It SHOULD work on other versions, at least on 2.x, but I have no idea right now what versions work and what don't. The fact I had to override a view probably don't help that, but I'll do my best when I have the time to test it in different versions with different SCM's and stuff ):

## Tests

For the tests to succeed, you'll have to run `rake test:scm:setup:all` before running the tests themselves.

## Contributors

As usually with my github stuff, I made this because it was useful for me but shared in case anyone else finds it useful. If you do want to contribute with anything, feel free to fork, make a pull request, create issues, anything you want.

## License

This plugin is licensed under the [MIT license](LICENSE)
