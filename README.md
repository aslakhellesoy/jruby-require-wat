Test case for [JRUBY-7097](http://jira.codehaus.org/browse/JRUBY-7097)

```
jruby -Ilib lib/wtf/wat.rb
```

That prints `WTF`. Wat.
On other rubies you'd get a `LoadError`, which is what you'd expect. There is no `libwtf.rb` file!

