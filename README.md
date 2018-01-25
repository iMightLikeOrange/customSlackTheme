# customSlackTheme
Some thing I took the trouble to make an account for


### This goes at the bottom of ssb-interop.js
```
document.addEventListener('DOMContentLoaded', function() {
  $.ajax({
   url: 'https://cdn.rawgit.com/iMightLikeOrange/customSlackTheme/<commit number>/slack.css',
   success: function(css) {
     $("<style></style>").appendTo('head').html(css);
   }
 });
});
```
