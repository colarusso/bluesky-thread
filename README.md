# A Tool for Unrolling and Inspecting Bluesky Threads

This tool adds thread unrolling to Simon Willison's [Bluesky Thread](https://github.com/simonw/tools/blob/main/bluesky-thread.html). Here's the [context behind Simon's html tools](https://simonwillison.net/2025/Dec/10/html-tools/). It also added collapse and expand behavior to the thread view. 

You can turn the code below into a bookmarklet at https://caiorss.github.io/bookmarklet-maker/ 

This lets you just click the bookmarklet when viewing a thread to see it unrolled or inspect the replies. 

```
javascript: (function() {
        var currentUrl = window.location.href;
        var openUrl = "https://colarusso.github.io/bluesky-thread/?url=" + encodeURIComponent(currentUrl);
        window.open(openUrl, '_blank');
})();
```

Alternativly, a bookmarklet can be found on the [GitHub Page](https://colarusso.github.io/bluesky-thread/).
