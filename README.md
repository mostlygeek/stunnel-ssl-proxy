# About

When I do development it is a pain to set up a web server that can handle HTTPS. Especially when I use node.js I want my development and my production code to be as close as possible. In production node listens on HTTP and a proxy in front provides SSL. 

Using `stunnel` gives a lightweight, simple to configure SSL endpoint for doing development. 

# Instructions 

## TL;DR

![too-lazy-to-read-3-steps](https://raw.github.com/mostlygeek/stunnel-ssl-proxy/master/screenshot.png)

## Step 1 - install stunnel

* On OSX, use macports. `sudo port install stunnel` 

## Step 2 - run create-cert.sh

* You will get prompted to enter a bunch of SSL cert info
* The only important one is the FQDN, use `localhost` if you're working off of the same machine

These values don't really matter as you're self signing your cert anyways. It'll no doubt fail browser security checks. 
So you can enter almost anything. You'll have to manually accept the certificate anyways. 

## Step 3 - 

Run `start-tunnel.sh`


