# Mailcatcher

[Mailcatcher](http://mailcatcher.me) catches mail and serves it through a dream.

Run with : `docker run -d -p 1025:1025 -p 1080:1080 --name mailcatcher jeanberu/mailcatcher`

Deliver mails to `smtp://127.0.0.1:1025` and check out [http://127.0.0.1:1080]() to see them.

## Change default arguments

To change options, replace Docker image default command. You can see option list
[here](https://github.com/sj26/mailcatcher#command-line-options).

Example: `docker run -d --expose 80 -p 80:80 -p 1025:1025 --name mailcatcher jeanberu/mailcatcher --ip=0.0.0.0 
--http-port=80`

Docker image's default options are: `--ip=0.0.0.0`.
