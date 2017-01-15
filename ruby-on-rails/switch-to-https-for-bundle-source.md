# Switch to HTTPS for Bundle Source

You might have something like this in your `Gemfile`:

```
gem "activeadmin", github: "activeadmin"
```

It will cause this warning you do `bundle`:

```
The git source `git://github.com/activeadmin/activeadmin.git` uses the `git` protocol, which transmits data without encryption. Disable this warning with `bundle config git.allow_insecure true`, or switch to the `https` protocol to keep your data secure.
```

In order to prevent this warning in the future, run this command to prevent it
globally:

```
bundle config --global github.https true
```

References:
* https://github.com/bundler/bundler/issues/4978#issuecomment-260141406
