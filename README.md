# jQuery Hash Plugin

Detailed article about this plugin: [here(Chinese)](https://blog.netsh.org/posts/jquery-hash-plugin_1455.netsh.html).

This plugin enables you to store tiny datas in the URL hash.

For example, you may want to save the preference of an webpage user interface in the hash like:

```
website.com/uri#;color=red;theme=vector
```

You got `;key=value` pairs in the URL hash, each one stating with a semicolon.

This is distinctive from using traditional question/& marks (?) in an url query string.

## How to use

Before using the plugin, you need to include the jQuery library.

```
<script type='text/javascript' src='https://ajax.aspnetcdn.com/ajax/jQuery/jquery-1.7.2.min.js'></script>
```

Then, include the hash plugin js file.

```
<script type='text/javascript' src='jquery.hash.min.js'></script>
```

## Basics

To store a new key=value pair, run script:

```
$.hash("key", "value");
```

To read the value of an existing key=value pair, run script:

```
$.hash("key");
// will return "value".
```

To modify the existing key=value pair, run script:

```
$.hash("key", "new-value");
```

To remove a key=value pair, run script:

```
$.hash("key", null);
```

You can always run the following code to clear out everything in the hash:

```
window.location.hash = '';
```

