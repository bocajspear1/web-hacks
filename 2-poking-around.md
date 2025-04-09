---
id: poking-around
title: Poking Around
previous_page: running-the-app
next_page: sql-injection
---

If you go to `localhost:1337` in your browser, you should get something like this:

![Main page of website](images/main-1.png)

To see how easy it is to modify PHP code and see changes, open the `app/index.php` file. Under the `</h2>` tag, insert the following:

```
<?php echo "hello hacking!"; ?>
```

Note that PHP code we just inserted and around the page must be surrounded by `<?php` and `?>`.

Refresh the page and note that the changes are in effect:

![Main page with changes](images/main-2.png)

Congrats, you've coded in PHP! Now remove the changes to get us back to a clean slate.