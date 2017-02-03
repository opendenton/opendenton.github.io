[![Stories in Ready](https://badge.waffle.io/opendenton/opendenton.github.io.png?label=ready&title=Ready)](http://waffle.io/opendenton/opendenton.github.io)

## [OpenDenton.com](https://www.opendenton.com/)

### Using functional includes

We've made some functional utilities for including dynamic content!

#### Images

```liquid
{% include image.html src="/assets/images/program-02.jpg" alt="Denton Texas" retina=1 %}

```
_args_

@retina | 1 or 0

_output:_
```html
<img src="http://127.0.0.1:4000/assets/images/program-02@2x.jpg" at2x="/assets/images/program-02@2x.jpg" alt="Denton Texas" width="412" height="234">
```


#### EZ Media Queries
##### _above()_
```sass
.class {
  key:value
  @include above(media) {
    key:value
  }
}
```
##### _below()_
```sass
.class {
  key:value
  @include below(media) {
    key:value
  }
}
```

_args_

media = _mobile_, _tablet_, _desktop_


### Notes

To-Do

- [ ] get info@opendenton.com forwarding to opendenton@gmail.com (for MailChimp)
