# EDBTpedia


* [Install Hugo](https://gohugo.io/getting-started/installing/)
  Note: you need to install the extended version.



## Run Local site

Just run

```bash
hugo server -D --port=8080 --bind=0.0.0.0
```

Notice that the `-D` flag is used to rendrer draft elements.

More information [here](https://gohugo.io/commands/hugo_server/)

## Build

Just run

```bash
hugo
```

More information [here](https://gohugo.io/commands/hugo/)

## Edit data

You can edit

* general information about the site into the `config.toml` file.
* some data into `data/*.yml` files, like header or footer information
* some content into `content/**` files.
* some static assets like images into the `static/*` folder


<!-- ### Publish

To publish the site on firebase, just run `firebase deploy`.
Note that you need to authenticate once with `firebase login`
YOU DON'T NEED to publish manually the website, it's already done by pushing on `develop` or `master` branches.
 
You could take a look at the `.gitlab-ci.yml` file


### Extract data from CFP -->

TODO...
