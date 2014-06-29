Instructions to contribute:

1) Download this repo:

```
$ git clone git@github.com:bayesimpact/bayesimpact.github.io.git
```

2) Checkout the `source` branch.

```
$ git checkout source
```

3) Install all necessary Ruby gems

```
$ bundle install
```

If you don't have Ruby > 1.9.3 installed (check with `ruby --version`), follow instructions [here](https://github.com/sstephenson/rbenv#installation) to get rbenv (a Ruby version manager) and to install Ruby 2.1.2. Then type in

```
$ gem install bundler
```

4) Finally, use this command to set up an automatic rake deploy task

```
rake setup_github_pages
```

In the prompt, enter `git@github.com:bayesimpact/bayesimpact.github.io.git`

Now you have a clone of the Octopress blog source that can create the master used to serve assets on the github page. When you make changes, make them on the `source` branch (or a branch off the `source`) branch. Then use this command:

```
rake deploy
```

to update the live site. It should take < 30 secs to see changes.