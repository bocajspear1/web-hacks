---
id: running-the-app
title: Running our App
previous_page: index
next_page: poking-around
---


# Running Our Application

**Expected Knowledge:** Some familiarity with coding and Linux, basics of HTTP, Docker (or Podman) is installed, you know how to use `git`

We will be using a web application I made in PHP with Docker on Linux. It's intentionally very vulnerable. If you're not familiar with the PHP language, the main things are:

- The language uses brackets
- Variables start with a dollar sign (`$`)
- Lines end with a semicolon (`;`)
- String concatination is done with periods (`.`)

For a more detailed description, you can read up on it [here](https://www.w3schools.com/php/). 

The nice part is that we can make edits to PHP and on next load of the page, the changes will be in effect. No need to restart anything. PHP code also lives in the same files as the HTML, so you don't have to have extra template files flying around.

You can get documentation on different PHP functions [at its website](https://www.php.net/docs.php). Usually searching `php <THING YOU WANT TO DO>` will get you results on search engines due to PHP being fairly old (it was made in 1995) and very well used.

## Prerequisites

You need to have Docker installed, [follow the instructions here](https://docs.docker.com/engine/install/). Ensure your user has permissions to use Docker otherwise you'll get `permission denied` errors.

You should also make `make` installed. This should come in many build tool packages and usually in a package called `make` in many Linux distros.

## Getting the Repo

Use `git` to grab a copy of the code:

```
git clone https://github.com/bocajspear1/super-cool-community.git
```

Then change into its directory:

```
cd super-cool-community
```

Then use `make` to run the Docker build process.

```
make build
```

Once this is done, you can run the application with:

```
make run
```

The vulnerable web application will be available on port `1337`.