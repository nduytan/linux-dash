<h1 align="center">
  <a href="https://linux-dash.github.io">
    <img src="https://raw.githubusercontent.com/afaqurk/screenshots/master/linux-dash/v2.0-logo.png"/>
  </a>
</h1>

<p align="center">
  <small>A simple & low-overhead web dashboard for linux systems</small>
</p>

<h4 align="center"><a href="https://linux-dash.github.io">linux-dash.github.io</a></h4>

<p align="center">
  <small>
    <a href="https://linux-dash.github.io/demo">Demo</a> &nbsp;|&nbsp;
    <a href="https://linux-dash.github.io/docs">
      Docs
    </a>
  </small>
</p>


<p align="center">
  <a href="https://gitter.im/afaqurk/linux-dash">
    <img
      src="https://badges.gitter.im/gitterHQ/gitter.png"
      alt="linux-dash Gitter chat">
  </a>
</p>

<br/>

## Features
* **Small** ----- Under 400KB on disk _(with .git removed)!
* **Simple** --- A minimalist, beautiful dashboard
* **Easy** ------ Drop-in installation
* **Versatile** - Choose your stack from Node.js, Go, C, Python, PHP, or Binary

## Installation

### Step 1
```sh
## 1. clone the repo
git clone --depth 1 https://github.com/linux-dash/linux-dash.git

## 2. go to the cloned directory
cd linux-dash/app/server

```
OR, if you prefer to download manually:

```sh
## 1. Download the .zip
curl -LOk https://github.com/afaqurk/linux-dash/archive/master.zip && unzip master.zip

## 2. navigate to downloaded & unzipped dir
cd linux-dash-master/app/server

```

### Step 2

See instructions for preferred server linux-dash server _(all included)_:

* [Node.js](#if-using-nodejs) _(recommended)_
* [Go](#if-using-go)
* [Python](#if-using-python)
* [C](#if-using-c)
* [PHP](#if-using-php)

<br/>
#### If Using Node.js
```sh
## install dependencies
npm install --production

## start linux-dash (on port 80 by default; may require sudo)
node index.js

```

<br/>
#### If Using Go
```sh
## start the server (on port 80 by default; may require sudo)
go run index.go
```

To build a binary, run `go build && ./server -h`. See [@tehbilly](https://github.com/sergeifilippov)'s notes [here](https://github.com/afaqurk/linux-dash/pull/281) for binary usage options

<br/>
#### If Using Python
```sh
# Start the server (on port 80 by default; may require sudo).
python index.py
```

<br/>
#### If Using C
```sh
# extract the c server source files
tar -jxvf c_server.tar.bz2 -C ./

# compile the binary
cd c_server && make

# Start the server (on port 80 by default; may require sudo)
./index
```

<br/>
#### If Using PHP
(TODO: Update PHP instructions with snippets for nginx & apache configs)

1. Make sure you have the `exec`, `shell_exec`, and `escapeshellarg` functions enabled
2. Point your web server to `app/` directory under `linux-dash`
2. Restart your web server (Apache, nginx, etc.)
  - For PHP + Apache setup follow the [Digital Ocean tutorial](https://www.digitalocean.com/community/tutorials/how-to-install-linux-dash-on-ubuntu-14-04).
  - For help with nginx setup, see [this gist](https://gist.github.com/sergeifilippov/8909839) by [@sergeifilippov](https://github.com/sergeifilippov).

## Support

For general help, please use the [Gitter chat room](https://gitter.im/afaqurk/linux-dash).

## Security

**It is strongly recommended** that all linux-dash installations be protected via a security measure of your choice.


linux-dash does not provide any security or authentication features.
