# EDBTpedia

EDBTpedia is based on DevFest Theme Hugo
For building and generating the pages, you need to install the extended version.
* [Install Hugo](https://gohugo.io/getting-started/installing/)



## Run Local site

It is recommended to run the site locally to see the changes.
After doing the changes, just run:

```bash
hugo server -D --port=1313 --bind=0.0.0.0
```

Notice that the `-D` flag is used to render draft elements.

More information [here](https://gohugo.io/commands/hugo_server/)

## Build

Just run the below command to generate `html` and `css` files for deployment:

```bash
hugo
```

More information [here](https://gohugo.io/commands/hugo/)

Copy the content of `public/*` to the webserver.
## Edit data

You can edit

* general information about the site into the `config.toml` file.
* some data into `data/*.yml` files, like header or footer information
* some content into `content/**` files.
* some static assets like images into the `static/*` folder


### Speakers
For adding a new speaker, you should create a file in `content/speakers/*.md`
A speaker should have these params:

```yaml
key: zsolt_istván
name: Zsolt István
id: zsolt_istván
feature: false
company: Technische Universität Darmstadt
city: 'City, Country'
photoURL: /images/speakers/zsolt_István.png
socials:
  - icon: home
    link: 'https://zistvan.github.io/' 
  - icon: twitter
    link: 'https://twitter.com/zistvan'
  - icon: github
    link: 'https://github.com/zistvan'
shortBio: "Short bio"
companyLogo: /images/speakers/company/company.jpg
```
The body of the file is used as a long bio.


### Sessions

For adding a new session, you should create a file in `content/sessions/*.md`
A session should have these params:

```yaml
key: big_sequence_management:scaling_up_and_out
title: 'Big Sequence Management: Scaling up and out'
id: pY6MCQBMfIYlIKfHdhL4
language: French
format: conference
conference: EDBT2021
tags: []
level: beginner
duration: 114
speakers:
  - karima_echihabi
  - kostas_zoumpatianos
  - themis_palpanas
videoId: Pl4JPZLZ2VQ
presentation: null
draft: false
```
The body of the file is used as the session's abstract.