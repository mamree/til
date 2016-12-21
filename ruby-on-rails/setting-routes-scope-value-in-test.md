# Setting Route's Scope Value in Test

If I have a scope in the route called slug, I'd put this code in the test:

```
class ActionView::TestCase::TestController
  def default_url_options(options = {})
    { slug: "" }
  end
end
```

References:
- https://github.com/rspec/rspec-rails/issues/255#issuecomment-24796864
