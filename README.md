ics.js
============

Now you can make calendar friendly files client-side.  It outputs .ics files, so the files are compatible with all modern calendar software (Outlook, Apple Calendar, Google, etc.)

How To Use
----------
Simply use invoke the object and use the functions...

	var cal = ics();
	cal.addEvent(subject, description, location, begin, end);
	cal.addEvent(subject, description, location, begin, end); // yes, you can have multiple events :-)
    cal.download(filename);

`begin` and `end` need to be formatted in a way that is friendly to `Date()`


Example
-------
* **[Demo](https://rawgit.com/adlst4/ics.js/demo/demo.html)**

```
<script>
	var cal = ics();
	cal.addEvent('Demo Event', 'This is an all day event', 'Nome, AK', '8/7/2013', '8/7/2013');
	cal.addEvent('Demo Event', 'This is thirty minute event', 'Nome, AK', '8/7/2013 5:30 pm', '8/7/2013 6:00 pm');
</script>
<a href="javascript:cal.download()">Demo</a>
```


Dependencies
------------
The tool uses 2 libraries from the following projects:
* [FileSaver.js](https://github.com/adlst4/ics.js/blob/master/FileSaver.js)
* [Blob.js](https://github.com/adlst4/ics.js/blob/master/Blob.js)


Supported Browsers
------------------

| Browser        | Dependancies |
| -------------- | ------------ |
| Firefox 20+    | [FileSaver.js](https://github.com/eligrey/FileSaver.js) |
| Firefox ≤ 19   | [FileSaver.js](https://github.com/eligrey/FileSaver.js), [Blob.js](https://github.com/eligrey/Blob.js) |
| Chrome         | [FileSaver.js](https://github.com/eligrey/FileSaver.js) |
| Chrome for Android v28+ | [FileSaver.js](https://github.com/eligrey/FileSaver.js) |
| IE 10+         | [FileSaver.js](https://github.com/eligrey/FileSaver.js)         |
| Opera Next     | [FileSaver.js](https://github.com/eligrey/FileSaver.js) |
| Opera < 15     | [FileSaver.js](https://github.com/eligrey/FileSaver.js), [Blob.js](https://github.com/eligrey/Blob.js) |
| Safari ≤ 6     | [FileSaver.js](https://github.com/eligrey/FileSaver.js), [Blob.js](https://github.com/eligrey/Blob.js) |


Credits
------------------
* [Travis Krause](https://github.com/nwcell)
* [Kyle Hornberg](https://github.com/khornberg)
* [Eli Grey](https://github.com/nwcell/eligrey)
