# A Tool for Unrolling and Inspecting Bluesky Threads

This tool adds thread unrolling to Simon Willison's [Bluesky Thread](https://github.com/simonw/tools/blob/main/bluesky-thread.html) HTML tool. Here's the [context behind Simon's tools](https://simonwillison.net/2025/Dec/10/html-tools/). It also added collapse and expand behavior to the thread view along with support for very very long threads. 

Additionally, it's rather opinionated about what should be shown, counting a thread as only the string of replies that immediatly follow a post made by that poster. This means you have to start with the first post in a "thread." It also means that you can work with a "thread" made by someone in the replies. If this isn't the behavior you want, please fork and have fun.

If you turn the code below into a bookmarklet at https://caiorss.github.io/bookmarklet-maker/ you can click the bookmarklet when viewing a thread to see it unrolled or inspect the replies. 

```
javascript: (function() {
        var currentUrl = window.location.href;
        var openUrl = "https://colarusso.github.io/bluesky-thread/?url=" + encodeURIComponent(currentUrl);
        window.open(openUrl, '_blank');
})();
```

Alternativly, a bookmarklet can be found on the [live GitHub Page](https://colarusso.github.io/bluesky-thread/).
